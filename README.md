# vendors
Interface for working with vendor database

### Data that needs to be tracked

- manufacturer (*ACME*)     
- product_line (*pumps*)  
- distributor (*Joe's Pumps*)  
- point_of_contact:  
    - first name      (*Joe*)  
    - last name       (*Smith*)  
    - phone number    (*555-555-5555*)  
    - email           (*joe@joespumps.com*)  

There may be more than one distributor for the manufacturer.
The manufacturer may not have more than one product_line, then we'll use None for it.


### Nested Dictionary

    vendors = {'ACME' : 
                  {'pumps' : 
                       [['Joe\'s Pumps',
                       'Joe',
                       'Smith',
                       '5555555555',
                       'joe@joespumps.com'],]
                   }
                }

### Database

???


### Objects with Methods and Attributes

- manufacturer
    - attr: product_line
    
- distributor
    - attr: point_of_contact  
