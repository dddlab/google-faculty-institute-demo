# Jupyter Notebook on Google Compute Engine VM

* Create Compute Engine VM  
  * Choose Machine type according to your budget
  * Choose `Debian GNU/Linux 10 (buster)` image (default)
  * Check `Allow HTTPS traffic`
* Connect to your VM by SSH
* Execute,
  ```bash
  bash -c "$(curl -fsSL https://raw.githubusercontent.com/dddlab/google-faculty-institute-demo/master/setup.sh)"
  ```
* Restart your session by logging out then back in
* Execute,
  ```bash
  cd google-faculty-institute-demo && \
      ./setup.sh
  ```
* Create password for Jupyter notebook
* Execute,
  ```bash
  # cd ~/google-faculty-institute-demo
  docker-compose up # debugging mode
  ```
  or 
  ```bash
  # cd ~/google-faculty-institute-demo
  docker-compose up -d # daemon mode
  ```
* Click your VM's `External IP` address button on GCP console or  
  Go to `https://[VM External IP address]` manually in your browser
* Bypass security warning created by our self-signed encryption key
