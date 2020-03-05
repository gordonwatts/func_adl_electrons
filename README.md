# func_adl_electrons
Shows a simple demo to look at Z->ee invarrient mass.

# Setup

In order for this demo to run you'll need a local working python environment and a `ServiceX` instance running.

## Your environment

1. Create an environment that runs python 3.7 (only place it has been tested).
1. `pip install -r requirements.txt`

## ServiceX

You should run version 0.2 of `ServiceX` or larger. At the time of this file being written, one had to punch holes through `kubernetes` in order to access the proper ports. The following commands will do the trick (replace the pod name with your pod name, of course).

```
kubectl port-forward servicex-integrated-testing-servicex-app-5f769fc64c-4pwg2 5000:5000 &
```