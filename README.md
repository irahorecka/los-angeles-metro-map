# LA_metro_map
A Jupyter notebook repository for plotting real-time LA Metro bus coordinates on a map.
<br><hr>
## **Introduction**<br>
```metro_mapping.ipynb``` and ```gif_generator.ipynb``` complement each other in:
1) Gathering images of real-time bus locations in Los Angeles, CA.
2) Converting these images to a gif.
<br><br>
<p align = 'center'>
<img src=https://im7.ezgif.com/tmp/ezgif-7-350d455fe9b7.gif alt="LA Metro bus gif"
    width=400><br>
</p>
<hr>

## **Python Setup**<br>
This script requires Python 3.5 and above. Please see ```requirements.txt``` for required Python libraries. Clone this repository and use ```pip``` to install the necessary libraries into your conda environment, like this:<br><br>
```pip install -r requirements.txt``` <br><br>
You will have to install two additional libraries to properly execute ```export_png()``` from the ```bokeh.io``` module:<br>
1) ```pip install selenium``` 
2) ```conda install -c conda-forge phantomjs```

<hr>

## **Running the Notebooks**<br>
Run ```metro_mapping.ipynb``` entirely and execute ```main()``` to start collecting images (which will accumulate in the ```./map_figs``` directory).
<br>```main()``` will run indefinitely. When you are satisfied with the accumulated images, click the *square button* at the top of the notebook to interrupt the kernel:
<br>
<p align = 'left'>
<img src=https://i.imgur.com/0GbrRqH.png alt="Interrupt kernel"
    width=300><br>
</p><br>


Then, run the entirety of ```gif_generator.ipynb```. Provide an appropriate name for your gif when prompted in ```main()```. This will create a .gif file of your .png images in the ```./gif_files``` directory.
<br>
<p align = 'left'>
<img src=https://i.imgur.com/USkyq0P.png alt="GIF progress bar"
    width=400>
</p>
<hr>

## **Notes**<br>
A .png file will range from 200kb - 240kb in size. Accumulating hours of images can lead to a large .gif file. For example, 12 hours of images could lead to a ~ 1 GB gif image.

Please let me know if you have questions.

***Fin***


