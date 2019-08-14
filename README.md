# Anime4K

Anime4K is a state-of-the-art open-source high-quality real-time anime upscaling algorithm that can be implemented in any programming language, anywhere.  

![Thumbnail Image](results/Main.png?raw=true)
*State of the art as of August 2019, this will unquestionably be outperformed very soon.*

#### Disclaimer: All art assets used are for demonstration and educational purposes. All rights to their original owners. If you (as a person or a company) own the art and do not wish it to be associated whatsoever with this project, please contact me and I will gladly take it down.

<br/>
<br/>

# HLSL Usage Instructions (MPC-BE with madVR)  
**Windows Only**  
[HLSL Installation](HLSL_Instructions.md)

# Java Usage Instructions (Standalone)
Currently unavailable.  
Unfinished, Still cleaning and commenting the code.  
[Java Installation](Java_Instructions.md)


<br/>
<br/>
<br/>
<br/>



# Psudo-Preprint Preview

[Read Full Preprint Here](Preprint.md)

B. Peng  
August 2019  

*Ad perpetuam memoriam of all who perished in the Kyoto Animation arson attack.*  

## Table of Contents

[Abstract](Preprint.md#abstract)  
[Introduction](Preprint.md#introduction)  
[Proposed Method](Preprint.md#proposed-method)  
[Results and Upscale Examples](Preprint.md#results)  
[Discussion](Preprint.md#discussion)  
[Analysis and Comparison to Other Algorithms](Preprint.md#analysis)  


## Abstract
We present a state-of-the-art high-quality real-time SISR alorithm designed to work with japanese animation and cartoons that is extremely fast *(~3ms with Vega 64 GPU)*, temporally coherent, simple to implement *(~100 lines of code)*, yet very effective. We find it surprising that this method is not currently used 'en masse', since the intuition leading us to this algorithm is very straightforward.  
Remarkably, the proposed method does not use any machine-learning or statistical approach, and is tailored to content that puts importance to well defined lines/edges while tolerates a sacrifice of the finer textures. The proposed algorithm can be quickly described as an iterative algorithm that treats color information as a heightmap and 'pushes' pixels towards probable edges using gradient-ascent. This is very likely what learning-based approaches are doing already under the hood (eg. VDSR<sup>**[1]**</sup>, waifu2x<sup>**[2]**</sup>).

[Read Full Preprint Here](Preprint.md#introduction)