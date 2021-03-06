# titan-gpu

George Ostrouchov, Don Maxwell, Rizwan Ashraf, Millikarjun Shankar, and James Rogers. 2020. GPU Lifetimes on Titan Supercomputer: Survival Analysis and Reliability. In Proceedings of the International Conference for High Performance Computing, Networking, Storage and Analysis (SC '20). Association for Computing Machinery, New York, NY, USA

- Data and code for SC20 paper about Titan GPU reliability analysis.
- Includes R code to generate graphics for paper and additional analyses
  - See code/README for instructions
- Includes original Titan GPU reliability data on over 100,000 collective hours of operation
  - data/titan.gpu.history.txt - history data
  - data/titan.service.txt - service nodes for exclusion
- Includes output data files produced by code/TitanGPUmodel.Rmd
  - data/gc_full.csv - cleaned up data (see paper and R code)
  - data/gc_summary_loc.csv - one record per GPU (variables: SN,time,nlife,nloc,last,col,row,cage,slot,node,max_loc_events,time_max_loc,dbe,dbe_loc,otb,otb_loc,out,batch,days,years,dead,dead_otb,dead_dbe) (see paper and R code)
- Includes .Rmd analysis document as TitanGPUmode.html
- Includes Python code to process data/gc_full.csv into graphics from time-between-failure analyses
  - See code/tbf-analyses/README for instructions