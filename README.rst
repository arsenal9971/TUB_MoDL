Daedalus Intensive Course - Tensorflow Session
==============================================
*05 December 2018*

**Intended for participants of the course**

.. contents:: Navigation

About this repository
---------------------

Here you find all the information and materials needed to follow the **tensorflow session**. During this session we will give a short introduction to the deep learning framework **Tensorflow** and use it to numerically investigate the implications of theoretical results concerning the approximation properties of deep ReLU neural networks. In particular, we will consider an observation concerning the relationship between the depth of a network, the regularity of the chosen acitvation function and the approximation properties of the network made by D. Yarotsky in the following paper:

- Yarotsky, D. (2017). Error bounds for approximations with deep ReLU networks. Neural Networks, 94, 103-114.

You can download the paper on `arxiv <https://arxiv.org/abs/1610.01145>`_ (see p. 28 for more details).


Requirements
------------

The session will provide possibilities to **interactively** experiment with some of the code snippets we provide here. If you want to actively participate you will need to have the software packages listed below **installed** on your system. The next section gives instructions about how to setup all the required packages using a **miniconda** virtual environment that you can (if you want to) easily remove from your system after the session. 

If you already have the required software installed, or you want to use a different installation method and know what you are doing: excellent. If not, simply follow the instruction of the next section.

Here is a list of what you will need:

- Python 3
- Tensorflow 
- Jupyter / IPython
- Scipy / Numpy
- Matplotlib / Pyplot


Installation instructions
-------------------------

1. Make sure you have a version of **Python 3** installed. You can find instructions on how to do it in the `Python wiki <https://wiki.python.org/moin/BeginnersGuide/Download>`_.

2. Install the **miniconda** package and environment manager. You can find instructions on how to do it in the `Conda documentation <https://conda.io/docs/user-guide/install/index.html>`_. Make sure to get the version for Python 3.

3. Create a new conda environment by running the following in your command line, respectively the Anaconda Prompt, if you are a Windows user (you can choose a different name for the environment if you want):

    .. code-block:: bash
        
        $ conda create --name dl_seminar python=3

4. Activate the newly created environment by running

    .. code-block:: bash
        
        $ conda activate dl_seminar

   (Try :code:`$ source activate dl_seminar` instead of :code:`$ conda activate dl_seminar` if this did not work.)

5. Install all the required Python packages within the new environment by running

    .. code-block:: bash
        
        $ conda install scipy
        $ conda install matplotlib
        $ conda install jupyter
        $ conda install tensorflow

6. To test if your Tensorflow installation was successful you can open Python 3 in a command line and run

    .. code-block:: python

        >>> import tensorflow as tf
        >>> print(tf.__version__)
        >>> session = tf.Session()

   If the Tensorflow version is printed correctly and creating the Tensorflow session prints out some additional version information but does not throw an error then you have sucessfully installed Tensorflow and are ready for the practical session.
