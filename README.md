# Beebotte_modul2.1
Vejledning i brug af Beebotte til at vise data fra eks RPI på hjemmeside

# Beebotte Python SDK can simply be installed using pip:

sudo pip3 install beebotte //On Linux

# Include the Beebotte SDK for Python
from beebotte import *

bclient = BBT("API_KEY", "SECRET_KEY")

## Create a Resource object
res1 = Resource(bclient, 'dev', 'res1')
## Write to the resource
res1.write('Hello World')

## Or simply
bclient.write('dev', 'res1', 'Hello World')

## Create a Resource object
res1 = Resource(bclient, 'dev', 'res1')
## Publish to the resource
res1.publish('Hello World')

## Or simply
bclient.publish('dev', 'res1', 'Hello World')
