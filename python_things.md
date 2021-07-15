Some stuff which can help in python prototyping

# Jupyter-lab on a remote server
Assuming you want to run jupyter-lab on a server to which you can ssh, and view the notebooks in your local browser
```bash
# Assuming you can ssh to a server with IP 10.10.10.10

# On the server (after ssh-ing) start the notebook on the desired port:
jupyter-lab --no-browser --port=8888
# this will give you the URL to access the lab

# On your local machine
ssh -N -L 8888:localhost:8888 user.name@10.10.10.10

# Now you can open in a browser the URL you got from the server
```
