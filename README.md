# SADFace
The Simple Argument Description Format

This is what a simple SADFace document looks like:

~~~~
{
    "analyst_email": "siwells@gmail.com", 
    "analyst_name": "Simon Wells", 
    "created": "2017-07-11T16:32:36", 
    "edges": [
        {
            "id": "d7bcef81-0d74-4ae5-96f9-bfb07031f1fa", 
            "source_id": "49a786ce-9066-4230-8e18-42086882a160", 
            "target_id": "9bfb7cdc-116f-47f5-b85d-ff7c5d329f45"
        }, 
        {
            "id": "f57ecb48-dfd5-4789-b3c5-46f770f4113d", 
            "source_id": "30c9c0ac-ddef-44e7-897d-52ffee97b837", 
            "target_id": "49a786ce-9066-4230-8e18-42086882a160"
        }, 
        {
            "id": "c48c3d75-a8b3-439a-9a2f-b987eaae2c9a", 
            "source_id": "02b4009b-1a12-4d53-ab3a-efabe6c44694", 
            "target_id": "49a786ce-9066-4230-8e18-42086882a160"
        }, 
        {
            "id": "86e797aa-ecb0-4fcd-8838-263ceedb099e", 
            "source_id": "5760a93a-55e7-447c-a245-7f8d7e7e4434", 
            "target_id": "02b4009b-1a12-4d53-ab3a-efabe6c44694"
        }, 
        {
            "id": "b2531a60-6559-4560-b57b-320f1f3b8386", 
            "source_id": "fbaa9b79-0965-45a1-9fd4-60701c2102cf", 
            "target_id": "5760a93a-55e7-447c-a245-7f8d7e7e4434"
        }
    ], 
    "edited": "2017-07-11T16:32:36", 
    "id": "94a975db-25ae-4d25-93cc-1c07c932e2f8", 
    "metadata": {}, 
    "nodes": [
        {
            "id": "9bfb7cdc-116f-47f5-b85d-ff7c5d329f45", 
            "metadata": {}, 
            "sources": [], 
            "text": "The 'Hang Back' campaign video should not have been published, and should be withdrawn.", 
            "type": "atom"
        }, 
        {
            "id": "49a786ce-9066-4230-8e18-42086882a160", 
            "name": "support", 
            "type": "scheme"
        }, 
        {
            "id": "30c9c0ac-ddef-44e7-897d-52ffee97b837", 
            "metadata": {}, 
            "sources": [], 
            "text": "The 'Hang Back' advert does not clearly express the intended message", 
            "type": "atom"
        }, 
        {
            "id": "02b4009b-1a12-4d53-ab3a-efabe6c44694", 
            "metadata": {}, 
            "sources": [], 
            "text": "The 'Hang Back' campaign was the wrong campaign to run", 
            "type": "atom"
        }, 
        {
            "id": "5760a93a-55e7-447c-a245-7f8d7e7e4434", 
            "name": "conflict", 
            "type": "scheme"
        }, 
        {
            "id": "fbaa9b79-0965-45a1-9fd4-60701c2102cf", 
            "metadata": {}, 
            "sources": [], 
            "text": "Road users have a responsibility to make our roads safer by being more vigilant.", 
            "type": "atom"
        }
    ], 
    "resources": []
}
~~~~

This is what the argument contained in that document looks like when exported to the Dot format:

![alt text](https://raw.githubusercontent.com/siwells/SADFace/master/examples/hangback/data.png "Extract from the Hang Back analysis")


## QuickStart

SADFace can currently be used in two ways, as a Python library, to builds SADFace documents from an existing argument tool, or as a command line app using the interactive argument when invoking the tool.

### Library

### Command Line Tool

Invoke the tool as follows: 

~~~~
 $ python src/sadface.py -i
~~~~

This will launch SADFace in interactive mode. If you have a config file then this can be passed in using the -c argument, e.g.

~~~~
 $ python src/sadface.py -c etc/simon.cfg -i
~~~~



