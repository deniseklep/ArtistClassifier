Classify artist based on the artworks 

Install virtual environment: 
In command line: 

virtualenv project_artworks
.\project_artworks\Scripts\activate
pip install tensorflow
pip install jupyter
pip install --upgrade pywin32==224 (currently not playing nice with tensorflow2 on windows)
pip install pandas
pip install matplotlib
pip install pillow

in Albrecht_Dürer folder, run from cmd or powershell:
get-childitem *.jpg | foreach { rename-item $_ $_.Name.Replace("Albrecht_Dürer", "Albrecht_Durer") }