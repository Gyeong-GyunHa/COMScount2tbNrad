!****************************************************************************
!*This Fortran code converts from COMS count value (Binary)                 *
!*                                     to temperature and radiance (ASCII). *
!*                                                                          *
!*INPUT                                                                     *
!*nx and ny : Array size of COMS data                                       *
!* FD :  1375 * 1429                                                        * 
!* ENH : 1934 * 1544                                                        *
!*Input units number 10 to 11 : Temperature and radiance conversion tables  *
!*Input units number 20 to 24 : COMS count data                             *
!*Each unit is assigned chanel in ascending order(IR1, IR2, WV, SWIR, VIS). *
!*Example code uses Jan 1, 2016, 02:45 UTC data.                            *
!*Input units number 40 (optional) : latitude and longitude conversion table*
!*                                                                          *
!*OUTPUT                                                                    *
!*chanel_tb.dat : Temperature of each chanel obtained from count value      *
!*chanel_rad.dat : Radiance of each chanel obtained from count value        *
!*Their unit numbers are 30 to 39.                                          *
!*                                                                          *
!*Optional commands                                                         *
!*There are several lines for additional analysis.                          *
!*Line number 42, 43 and 154 to 162 are commented.                          *
!*If users want to know latitude and longitude of each cell,                *
!*                                     relevant to same row of latticepoint.*
!*Each column of latticepoint denotes column number and row number of cell. *
!*And each column of latlon represents latitude and longitude of cell,      *
!*                                     relevant to same row of latticepoint.*
!*                                                                          *
!*Author : Gyeong-Gyeun Ha                                                  *
!*Affiliation : National Meteorological Satellite Center (of KMA)           *
!*Date: Nov.2016                                                            *
!****************************************************************************