# Heat_equasion
Heat equasion solution modeling  
Linear - dT/dt=l*d^2(T)/dx^2 
conditions:  
t=0 T=0  
x=0 T=T_0=const  
x=L T=0  

Model solution - T(q)=1-2/sqrt(pi)*int(exp(-c^2)dc)  [c from 0 to q=x/2sqrt(l*t)] 

Nonlinear - dT/dt=d/dt(l(T)*dT/dx)  
conditions:
t=0 T=0  
x=0 T(0,t)=T_0*t^(1/sigma)  T_0=const  sigma=const  
x=L T=0  

Model solution -   
if (x<=ct) T(x,t)=(sigma*c*(c*t-x)^(1/sigma))/lambda_0  
else T(x,t)=0

The solutions were calculated with Explicit scheme and Implicit Six-Point weighted scheme  
