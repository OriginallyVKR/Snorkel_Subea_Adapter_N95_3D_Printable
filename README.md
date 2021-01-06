# Snorkel_Subea_Adapter_N95_3D_Printable
This repo consists of the CAD designs of the adapter to convert a Decathlon - SUBEA snorkelling mask to be used as an N95 Mask for medical personnel. awe designed during the 


# Introduction 

<p>To prevent transmission of the novel SARS-CoV-2 virus among exposed health care workers (HCW), the WHO recommends the use of tight-fitting facepiece respirators such as the FFP2 or N95.1  However, global personal protective equipment (PPE) stockpiles are shrinking rapidly because of the elevated demand during the COVID-19 pandemic and since the capacity to expand PPE production is limited while supply chains are disrupted and counterfeit deliveries discovered, severe local shortages of trustworthy respirators are a reality.2-4  Possible deconfinement measures are likely to increase demand even further as indications to wear respirators become broader (i.e. semi-urgent surgery for affected COVID-19 patients)<sup>[<a href="https://www.researchgate.net/publication/341666605_Verification_of_two_Alternative_Do-it-yourself_Equipment_Respirators_Seal_as_COVID-19_Protection_VADERS-CoV_a_quality_assessment_pilot_study">source</a>]</sup>. 
  
  We aimed at mitigating the shortage of respirators with do-it-yourself Respirator (ADR) with components found in most hospitals - using a CPAP inline filter (using the appropriate filter - N-95, HEPA etc).
 
 On research we discovered that there was a snorkelling mask (sold by Decathlon - <a href="https://www.decathlon.in/p/8573237/easybreath-full-face-mask/adult-snorkeling-mask-easybreath-500-blue">ADULT SNORKELING MASK EASYBREATH 500</a>  )</p> which were readily available in most stores in our demographic (Bangalore, India), we then set out trying to design an adapter to connect the snorkelling mask to a CPAP inline filter. 
 
 # Design description
 
 <p> We started by exploring designs that were available in the open-source domain and landed a couple of adapters. We were fortunate enough to be able to source an FDM based 3D printer. The designs we found required support structures to be printed and had an average print time of 12 hours (15% infill) - the real challenge was once the print was done - post processing was a nightmare as the structure was such that it didnt allow us to clean up support material from the inner cavities. 
  
  We tried multiple orientations to reduce the support structures but were in no luck - the design by default was only available as STL files and gave us little flexibility to modify the wall thickness. The reason we wanted to alter the wall thickness was to increase our production rate, we wanted to be able to churn out 30 units in 3 days and the design didnt allow us to do this. Additionally, the adapter wasn't to operate at high pressure, we weren't looking at putting the adapter through any pressure higher than 14cmH2o (0.013bar or 1.199psi). 
  
  We soon realised that we had to start from scratch and brought in the  <a href="https://www.decathlon.in/p/8573237/easybreath-full-face-mask/adult-snorkeling-mask-easybreath-500-blue"> snorkelling</a> and the N95 CPAP filter, got the dimensions measured and designed the adapter. 
  
  With the newer design, we were able to print the adapter with no support (this was possible as we had redesigned the neck with lesser inclination, which allowed the printer to print subsequent layers with no underlying support as the layers weren't steep enough to warrant underlying support)
  
 PFB the drawings of the adapter and a preview of the adapter on the slicer. 
 
 
 # Printer settings
 
 We used an FDM based printer with the following settings:

 * Material : PLA (polylactic acid) of 1.75mm red colour
 * Nozzle configuration : single nozzle 0.5mm
 * Infill : 15%
 * Speed : 100%
 * Supports : None
 * Z offset : None
 * Placement : placed flat with the wider mouth on the build plate (Refer image)
 
 Image from slicing software (we used Astro print <a href="https://cloud.astroprint.com/account/login"> Astroprint</a> as the slicer.
 
![Screenshot from 2021-01-05 21-08-51](https://user-images.githubusercontent.com/55281142/103667200-a44d8100-4f9b-11eb-8b00-af0bc61ae8fa.png)
 
 The print time was close to 4.5/5 hours at the above-said configuration for a single unit, we then replicated this and generated a 5 unit configuration to print at scale. The results were as follows:
 
 ![Final_part_monoaxial](https://user-images.githubusercontent.com/55281142/103777928-9b21ea00-5057-11eb-9788-bb4f7b356c0a.jpeg)

On connecting the CPAP inline N95 filter the results were as following:

![Connected_final_monoaxial](https://user-images.githubusercontent.com/55281142/103778038-b3920480-5057-11eb-949c-3076c6655905.jpeg)

We then printed about 5 as described earlier :

![5_final__monoaxial](https://user-images.githubusercontent.com/55281142/103778447-429f1c80-5058-11eb-9a71-e0751d26a0a2.jpeg)

Images of doctors using it in on field:

![Field_use_monoaxial](https://user-images.githubusercontent.com/55281142/103778516-5c406400-5058-11eb-997b-d1c3266e7165.jpeg)
  
# Licenses 
  
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Snorkel_Subea_Adapter_N95_3D_Printable</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Vishnu Ramakrishnan & Ateeb Hafeez</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/OriginallyVKR/Snorkel_Subea_Adapter_N95_3D_Printable" rel="dct:source">https://github.com/OriginallyVKR/Snorkel_Subea_Adapter_N95_3D_Printable</a>. 

# Contact us

For any queries additional you can write to us at vishnu.cats@gmail.com. 
