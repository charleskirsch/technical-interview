## Brand the Service Portal to your liking.

I updated the color scheme to something light and readable. I added a logo and banner image as well.

## Create a new Incident Record Producer for an end user and ensure the Service Portal links to it from the homepage.

I thought about this one from the perspective of a company that wants a less "IT" feeling form with a focus on simplicity.
The fields have more natural sounding questions and answers, using the built-in hint text.
All the fields map to Incident fields, and the two dropdowns map to Impact and Urgency using numbers as values.
If I wanted to add more to this I would create a message or popup if the user selected that work was stopped and it affected everyone directing them to call the service desk, and it would also cancel form submission. I wouldn't recommend allowing end users to submit an incident that would be prioritised as critical.

## Create a new Service Catalog item for a device of your choosing that requires Manager approval and generates two Catalog Tasks after approval is received. 

I created an iPhone 12 catalog item with a nice image and description.
The workflow creates two parallel tasks for shipping the phone and setting up the cellular plan.
I did this to demonstrate a join in a workflow to wait for both tasks to complete.

## Publish 3 Knowledge base Articles and ensure these can be browsed to in the Service Portal.

I created, published, and approved 3 articles in different categories with boilerplate text.
I also added them to the update set using the Add to Update Set utility from Share.

## Create a new Task type table and form showing at least the following fields: Number, Business Service, Configuration Item, Change Request (Reference to the change_request table), Knowledge Checkbox, State (Open, In Progress, Complete), Impact, Assignment Group, Assigned to, Short Description and Description.

I extended the Task table as a new table called "Test Task".
I added the following fields:
* Business Service - u_business_service (referencing cmdb_ci_service)
* Change Request - u_change_request (referencing change_request)

I added logic as necessary to address the asks in the test document.
The client scripts used to append data to the description field use callback functions.