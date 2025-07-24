## Robotic-Food-Sorting-System
This robot sorts food boxes placed on the ground. It uses a barcode to know the type of food, then sends it to the right conveyor belt. Another robot takes the boxes from the conveyor and puts them on the correct shelf. The robot works automatically, but a human can help if there is a problem.

## Execution Algorithm
- The robot system starts and checks that all sensors are functioning properly.

- The fixed robotic arm picks up the first food box from the ground.

- The robot scans the barcode attached to the box to determine its category.

- The item is classified into one of the following categories:

  Category 1: Canned goods

  Category 2: Bagged items

  Category 3: Frozen items 

- The box is placed onto the appropriate conveyor belt based on its category.

- If the barcode cannot be read or an issue is detected:

- The item is redirected to a special "obstacle" conveyor.

- A notification is sent to the supervisor.

- The robot repeats the process for the next item.

- If a conveyor belt becomes full, the robot pauses until the second robot clears space.

- Once space is available, the robot resumes operation automatically.

- In case of an unexpected error or emergency, the system sends an alert and stops temporarily.

## Working Envelope
| Element               | Description                                                                   |
| --------------------- | ----------------------------------------------------------------------------- |
| Robot Type            | Fixed robotic arm                                                             |
| Main Function         | Classify and sort food boxes by reading barcodes                              |
| Classification Method | Barcode scanning                                                              |
| Transport Method      | Conveyor belts assigned per category                                          |
| Environment           | Ground-level warehouse with boxes and 3+1 conveyors (including obstacle belt) |
| Human Supervision     | Only in emergency or alert situations                                         |
| Obstacle Handling     | Redirects item to obstacle path and notifies supervisor                       |


## Additional Notes
The robot operates autonomously without human intervention in normal conditions.

If any issue arises, the affected box is isolated, and the process continues without delay.

The system is scalable and can support more categories in the future if needed.
