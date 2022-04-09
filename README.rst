=======================================================================
Time frequency transforms under the mathematical framework of frames
=======================================================================


* Free software: MIT license

Installation
============

::

    pip install Time-Frequency-Analysis

You can also install the in-development version with::

    pip install https://github.com/nnanos/Time_Frequency_Analysis/archive/main.zip



Usage
=============

::

For each transform you can test the properties below:   
#. execution time 
#. perfect reconstruction property 
#. visualization

Steps to follow:

#. Clone the repo
#. change your path to /repo_dir/src/Time-Frequency-Analysis
#. Examples of execution:

    For NSGT_CQT : python __main__.py --front_end NSGT_CQT -p "{ ksi_s : 44100 , ksi_min : 32.07 , ksi_max : 3907.07 , B : 12 , matrix_form : 1 }" --plot_spectrograms True  
   
    For NSGT_scale_frames :   python __main__.py --front_end NSGT_SCALE_FRAMES -p "{ onset_det : False , ksi_s : 44100 , min_scl : 128 , ovrlp_fact : 0.5 , middle_window : np.hanning , matrix_form : 0 , multiproc : 1 }" --plot_spectrograms True
   
    For STFT : python __main__.py --front_end STFT -p "{ a : 1024 , M : 4096 , support : 4096 }" --plot_spectrograms True



Documentation
=============
