# Nowcasting for hands-on session OWM Academy
Three exercises to get familiar with radar data and nowcasting.

# Pre-requisites for the “hands-on session”

The exercises in this session will be done by using Google Colab notebooks, which ensures that you are all going to use the same Python version. Therefore the attendees are expected to create a Google account before the session and copy the example notebooks to their Google Drive. The material will be provided in the [GitHub repository](https://github.com/RubenImhoff/nowcasting-hands-on-OWM-academy).

## 1. Create a Google account

If you don't yet have a Google account, create it [here](https://accounts.google.com/signin/v2/identifier?flowName=GlifWebSignIn&flowEntry=ServiceLogin).

## 2. Install Google Chrome

For the best experience, we recommend using [Google Chrome](https://www.google.com/chrome) for this session. [Firefox](https://www.mozilla.org), [Microsoft Edge](http://www.microsoft.com/en-us/windows/microsoft-edge) and [Safari](http://www.apple.com/safari) should also work, but they might not support all functionalities needed for using the Google services.

## 3. Clone GitHub Repositories and copy notebooks to Colab

This step is required for running the Colab notebooks shared through the [GitHub repository](https://github.com/RubenImhoff/nowcasting-hands-on-OWM-academy). Sign in to your Google account, go to [Colab](https://colab.research.google.com/?utm_source=scs-index) and run the following commands in a new notebook.

    # mount your Google drive to access it from Colab
    import os
    from google.colab import drive
    drive.mount("mnt")
    %cd mnt/MyDrive
    # clone the repository from GitHub
    !git clone https://github.com/RubenImhoff/nowcasting-hands-on-OWM-academy.git
    # create notebook directory (if it doesn't already exist)
    if not os.path.exists('Colab Notebooks'):
        !mkdir 'Colab Notebooks'
    # copy the course notebooks to the above folder
    !cp nowcasting-hands-on-OWM-academy/notebooks/*.ipynb 'Colab Notebooks'

Now you can open the example notebooks in Colab by either navigating through your 'Colab Notebooks' folder or by uploading them if you have stored them locally.
