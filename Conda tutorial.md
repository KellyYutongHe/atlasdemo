# Conda Tutorial [ft. Patrick Liu & Erik Rozi]  
1. Download anaconda bash script in tmp folder on Atlas home directory. For most recent version, download from https://www.anaconda.com/distribution/  
`cd /atlas/u/<CSID>`  
`mkdir tmp`  
`cd tmp`  
`curl -O https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh`  


2. Validate the checksum using the Anaconda website if possible  
`sha256sum Anaconda3-2020.11-Linux-x86_64.sh`  


3. Run the installer (type yes and ENTER when prompted)  
`bash Anaconda3-2020.11-Linux-x86_64.sh`  


4. Follow the terminal instructions to accept license terms and confirm installation location  
  

  

5. Be patient. Very patient.  
6. Scream for help in the computer_cluster channel on Slack if necessary  


7. Activate installation using  
`source ~/.bashrc`  


8. Test installation using  
`conda list`  


9. Remove tmp folder  
`cd ..`  
`rm -R tmp`  


10. Set up conda environment (replace `version-num` with python version, or omit `=version-num` for default. As of this tutorial, default is python 3.9.2).  
`conda create --name name-of-environment python=version-num`  


11. Activate environment  
`conda activate name-of-environment`  


12. Install packages needed for project  
`conda install name-of-package`  


13. Deactivate environment when finished coding  
`conda deactivate`  





Installation help received from 
https://www.digitalocean.com/community/tutorials/how-to-install-anaconda-on-ubuntu-18-04-quickstart