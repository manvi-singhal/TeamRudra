# TeamRudra

The pattern was recognised to be the floating part of the digits of pi ( $\pi$ = 3.141592653589... )

The best way to find the digits was by [John Machin's formula](https://www.craig-wood.com/nick/articles/pi-machin/):
    
   $π/4 = 4cot⁻¹(5) - cot⁻¹(239)$
   
   $= 4tan⁻¹(1/5) - tan⁻¹(1/239)$
    
   $= 4 * arctan(1/5) - arctan(1/239)$
    
In order to obtain n digits, I have used fixed-point arithmetic to compute $\pi$ × 10<sup>n</sup> as a regular integer

We get:

  $arctan(1/x) = \frac{1}{x} - \frac{1}{3x^3} + \frac{1}{5x^5} - \frac{1}{7x^7} + \frac{1}{9x^9} - \cdots ( x >= 1 )$
  
  
  
  ### Run Code:
  
    1> c(pattern).
  
    2> pattern:pi(100).
