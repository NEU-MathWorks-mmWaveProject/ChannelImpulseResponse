# ChannelImpulseResponse
##  Description:
 
  The purpose of this project is to provide a plot of the Chanel Impulse Response
  in a use-case scenario of your choice.  This folder provides a Matlab function
  and an example of using it.

  The "getCIR.m" function imports the CIR values generated by a ray tracer.  In our
  case, it is the Wireless InSite from Remcom. 

  The example file "exampleGetCIR.m" shows how the Matlab function can be used in
  conjunction with few input files delivered in this package.


##  Matlab Function Description:

  The function extracts the received power values as well as the phase values provided
  at the output of a ray tracer and generates two plots (Rx power vs. time, and phase
  values vs. time).

  The only input requirements are the file containing these values and the receiver
  sensitivity threshold. The received power levels and phase values of the multipath
  components arriving at the receiver can be obtained via measurements using channel
  sounders and various antennas, or can be estimated with a ray tracer. The data
  organization in the input files is described in the header portion of the
  "getCIR.m" Matlab function.



##  Example Description:
  
  The "exampleGetCIR.m" file shows how we can use the "getCIR.m" Matlab function
  by applying one of the input files delivered in this folder. The input files refer
  to an indoor use-case scenario - a customizable conference room.

  The "CIR" folder contains four ".p2m" files generated by the ray tracer for the
  indoor scenario.  They represent various room configurations, from a complex scenario
  full of furniture and electronic equipment down to an empty room.

  The user can also generate his/her own input files for different use-case scenarios,
  and can process these files with the same "exampleGetCIR.m" file by changing the code
  to call for the appropriate input file names.  
  
  ## Acknowledgements
  This work is supported in part by MathWorks under the Development-Collaboration Research Grant
