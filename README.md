# utl-optimum-number-of-clusters-elbow-plot
Optimum number of clusters elbow plot
    Optimum number of clusters elbow plot                                                                                    
                                                                                                                             
    github                                                                                                                   
    https://tinyurl.com/y2hhsp2u                                                                                             
    https://github.com/rogerjdeangelis/utl-optimum-number-of-clusters-elbow-plot                                             
                                                                                                                             
    SAS Forum                                                                                                                
    https://tinyurl.com/y4g3p55v                                                                                             
    https://communities.sas.com/t5/New-SAS-User/how-to-plot-elbow-graph-INDEX/m-p/580612/highlight/true#M13583               
                                                                                                                             
    This is an remakable post!!                                                                                              
    https://tinyurl.com/y2hhsp2u                                                                                             
    https://stackoverflow.com/questions/15376075/cluster-analysis-in-r-determine-the-optimal-number-of-clusters/15376462     
                                                                                                                             
    Ben Profile                                                                                                              
    https://stackoverflow.com/users/1036500/ben                                                                              
                                                                                                                             
    *_                   _                                                                                                   
    (_)_ __  _ __  _   _| |_                                                                                                 
    | | '_ \| '_ \| | | | __|                                                                                                
    | | | | | |_) | |_| | |_                                                                                                 
    |_|_| |_| .__/ \__,_|\__|                                                                                                
            |_|                                                                                                              
    ;                                                                                                                        
                                                                                                                             
    data sd1.have;                                                                                                           
      input x  y  @@;                                                                                                        
      if 6 < y < 15 then delete;                                                                                             
    cards4;                                                                                                                  
      2.14 -1.68  0.30  2.70  2.62 -0.17  1.32 -0.75 -0.91 -0.39  1.98 -0.54  0.07                                           
     -1.47 -0.05  3.01  1.07 -0.05  1.13  1.28  1.56  1.56 -0.10  1.58  0.13  0.24                                           
      1.97  2.54  0.44  0.25 -0.54  0.76  1.95  2.39  2.75  2.94  5.25  1.32  3.56                                           
      3.18  1.64  1.99  5.05  2.54  1.85  2.14  3.23  1.93  1.87  1.60  3.00  2.18                                           
      5.39 -0.05  4.43  3.23  2.48  2.10  2.37  0.70  3.53  2.52  1.86  3.27  3.64                                           
      2.02 -0.08  1.65  1.41 -0.14  1.10  1.92 -0.12  3.80  2.79  0.15  0.78  2.30                                           
      0.01  1.19  2.09 -0.08  1.30  2.46  1.46  1.54  1.94  0.87  0.13  0.93  1.16                                           
      2.40  1.14  2.41  1.73  1.42  2.17 11.10  2.69 11.41  1.63 10.34  3.49  9.17                                           
      1.08 11.91  3.31  9.74  0.70 10.62  0.65  9.72  2.11 10.67  2.34  9.16  2.44                                           
      9.45  2.78 11.72  1.16 11.36  0.61 11.32  1.89 11.36  2.43 12.62  9.55 21.13                                           
      9.11 23.81 12.17 21.93  9.93 20.66  9.49 21.78 10.95 19.81  9.26 19.12  8.38                                           
     20.02 11.65 21.00  9.95 21.65 11.00 19.81 11.08 20.29 11.23 19.52  8.44 20.83                                           
     11.43 21.23 11.89 21.92 26.06 35.36 24.53 34.35 24.69 35.89 27.55 35.53 25.82                                           
     35.39 25.75 35.58 25.35 34.47 24.12 35.19 26.50 36.61 27.26 35.44 26.99 36.81                                           
     26.17 35.88 24.39 34.78 27.06 33.21 25.37 36.26 25.48 35.02                                                             
    ;;;;                                                                                                                     
    run;quit;                                                                                                                
                                                                                                                             
                                                                                                                             
    Up to 40 obs SD1.HAVE total obs=80                                                                                       
                                                                                                                             
    Obs      X        Y                                                                                                      
                                                                                                                             
      1     2.14    -1.68                                                                                                    
      2     0.30     2.70                                                                                                    
      3     2.62    -0.17                                                                                                    
      4     1.32    -0.75                                                                                                    
      5    -0.91    -0.39                                                                                                    
      6     1.98    -0.54                                                                                                    
      7     0.07    -1.47                                                                                                    
     ...                                                                                                                     
                                                                                                                             
     Y |                                                                                                                     
       |                                                                                                                     
    40 +                                                                                                                     
       |                                   * *                                                                               
       |                                  *****                                                                              
       |                                     *                                                                               
    30 +                                                                                                                     
       |                                                                                                                     
       |                   *                                                                                                 
       |                   ** *                                                                                              
    20 +                  *****                                                                                              
       |                                                                                                                     
       |                                                                                                                     
       |                                                                                                                     
    10 +                                                                                                                     
       |                                                                                                                     
       |          *                                                                                                          
       |          ******                                                                                                     
     0 +         ***** *                                                                                                     
       |          * *                                                                                                        
       |                                                                                                                     
       |                                                                                                                     
    10 +                                                                                                                     
       |                                                                                                                     
       -+---------+---------+---------+---------+-                                                                           
       -10        0        10        20        30                                                                            
                                                                                                                             
    *            _               _                                                                                           
      ___  _   _| |_ _ __  _   _| |_                                                                                         
     / _ \| | | | __| '_ \| | | | __|                                                                                        
    | (_) | |_| | |_| |_) | |_| | |_                                                                                         
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                        
                    |_|                                                                                                      
    ;                                                                                                                        
                                                                                                                             
    WANT total obs=15                                                                                                        
                                                                                                                             
       WITHIN                                                                                                                
       CLUSTER                                                                                                               
       SUM SQUARES  CLUSTERS                                                                                                 
                                                                                                                             
       22680.45        1                                                                                                     
        3845.63        2                                                                                                     
         258.85        3 ** optimum                                                                                          
         190.93        4                                                                                                     
         141.72        5                                                                                                     
         203.77        6                                                                                                     
       ...                                                                                                                   
                                                                                                                             
    Within                                                                                                                   
    Sum of Squares                  Optimum                                                                                  
           1             2             3             4             5                                                         
    30000 ++-------------+-------------+-------------+-------------+ 30000                                                   
          |                            |                           |                                                         
          |                            |                           |                                                         
          |                            |                           |                                                         
          |*   Within Cluster          |                           |                                                         
          | \  Sum of Squares          |                           |                                                         
    20000 +  \                         |  3 Clusters is Optimum    + 20000                                                   
          |   \                        |                           |                                                         
          |    \                       |                           |                                                         
          |     \                      |                           |                                                         
          |      \                     |                           |                                                         
          |       \                    |                           |                                                         
          |        \                   |                           |                                                         
    10000 +         \                  |                           + 10000                                                   
          |          \                 |                           |                                                         
          |           \                |                           |                                                         
          |            \               |                           |                                                         
          |              *.            |                           |                                                         
          |                 - .        |                           |                                                         
          |                     - .    |                           |                                                         
        0 +                         ^ -*-------------*-------------* 0                                                       
          -+-------------+-------------+-------------+-------------+                                                         
           1             2             3             4             5                                                         
                                                                                                                             
                                   CLUSTERS                                                                                  
                                                                                                                             
    *          _       _   _                                                                                                 
     ___  ___ | |_   _| |_(_) ___  _ __                                                                                      
    / __|/ _ \| | | | | __| |/ _ \| '_ \                                                                                     
    \__ \ (_) | | |_| | |_| | (_) | | | |                                                                                    
    |___/\___/|_|\__,_|\__|_|\___/|_| |_|                                                                                    
                                                                                                                             
    ;                                                                                                                        
                                                                                                                             
    %utl_submit_r64('                                                                                                        
    library(haven);                                                                                                          
    library(SASxport);                                                                                                       
    have<-read_sas("d:/sd1/have.sas7bdat");                                                                                  
    wss <- (nrow(have)-1)*sum(apply(have,2,var));                                                                            
    for (i in 2:15) wss[i] <- sum(kmeans(have,                                                                               
        centers=i)$withinss);                                                                                                
    want<-as.data.frame(wss);                                                                                                
    write.xport(want,file="d:/xpt/want.xpt");                                                                                
    ');                                                                                                                      
                                                                                                                             
    libname xpt xport "d:/xpt/want.xpt";                                                                                     
    data want;                                                                                                               
      set xpt.want;                                                                                                          
      clusters=_n_-1;                                                                                                        
    run;quit;                                                                                                                
    libname xpt clear;                                                                                                       
                                                                                                                             
    options ps=32;                                                                                                           
    proc plot data=want (where=(clusters<6));                                                                                
      plot wss*clusters="*"/href=3 box;                                                                                      
    run;quit;                                                                                                                
                                                                                                                             
                                                                                                                             
