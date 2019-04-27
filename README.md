# ML_project_Comp2

For docker instructions, can also see: https://github.com/bencammett/scikit-hep-examples
(forked from rappoccio/scikit-hep-examples)

Install Docker: https://docs.docker.com/install/

Clone repo:
```
$: git clone https://github.com/bencammett/scikit-hep-examples.git
```

Make scikit-hep directory and set up docker files:
```
$: cd scikit-hep-examples
$: docker pull srappoccio/scikit-hep-examples:latest
```

Docker is working in virtual machine, will need parallel directory to scikit called results:
```
$: mkdir ../results
```

Then, to run, execute:
```
$: ./runDockerX11OSX.sh srappoccio/scikit-hep-examples:latest
```

And in your internet browser, go to: http://127.0.0.1:8888

Once that page is loaded, terminal will output a line with "token=..." -- copy & paste the token into the corresponding field on the laoded browser page

In /results you will need the jupyter files you wish to run (for example, a .ipynb file in this repo) as well as any data files they may be reading from

**Important:** Any file that you with to save / are working on must be stored in the /results directory or it will be gone when you exit docker

