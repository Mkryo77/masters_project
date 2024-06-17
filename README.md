This repository is dedicated to showcasing the highlights from my masters project for my MPhys Physics and Astronomy Degree at Durham University. The project is titled "Plant Species and Pathogen Identification with Reflectance Spectra, UAV Imagery and Machine Learning" and my goal was to develop a remote method of classifying species of plants and assessing their health using just a few measurements of reflectance off of their leaves. To do this I was supplied with a dataset consisting of 798 mangrove trees, with this being split amongst three different species in the ratio: 250 red, 218 white and 330 black. Initially, I attempted to solve this problem using a manual statistical approach before bringing in machine learning algorithms to see if any improvements on the results could be made. The machine learning algorithm that I decided was best fit for this was neural networks which I made using PyTorch.

My code for solving the manual statistical approach can be found in - full_array.ipynb.
A video tour of the 3D plot showing the best possible approach to discriminating between the three species of mangroves according to a manual statistical approach can be seen in this video on Youtube: https://www.youtube.com/watch?v=cl525SBrMpg.

My code for my neural network practice can be found in - nn_learning.ipynb.

My code for my first attempt at creating a working neural network to distinguish between the different species can be found in - species_neural_network.ipynb.

I had to give a 20 minute presentation infront of an audience of approximately 20 people (including students and lecturers) and the slideshow for this can be found in - Project Talk.pptx

I then had neural networks which took one input and two outputs to distinguish between each species and health status individually. These had a variant which would try all wavelengths and then a second variant which focused specifically on opitcal wavelengths (as the technology for optical wavelengths is better than IR despite IR giving statistically better results so need to look into optical when considering the real-life application of my results).
To find Red mangroves:
  All wavelengths: nn_1in_2out.ipynb
  Optical only: nn_1in_2out_red_optical.ipynb

To find White mangroves:
  All wavelengths: nn_1in_2out_white.ipynb
  Optical only: nn_1in_2out_white_optical.ipynb

To find Black mangroves:
  All wavelengths: nn_1in_2out_black.ipynb

To distinguish between healthy and stressed red mangroves:
  nn_red_h_s_1in_2out.ipynb

To distinguish between healthy and stressed black mangroves:
  nn_black_h_s_1in_2out.ipynb

(White had no stressed mangroves so was not apart of the healthy vs stressed investigation)

To ensure my results could be applied practically I modelled the effect that the changing apparent brightness of the Sun at different times throughout the day had on the results which allowed me to calculate a percentage error (or confidence level) on the results I obtained. This model can be found in - solarlumination.ipynb.

To complete the project, I wrote a 30 page (+ appendices) research paper which can be found in - Mark_Ryan_Final_Report.pdf.
