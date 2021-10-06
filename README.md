# cisco-paketracer-SME-

# cisco-packet-tracer
The aim of this project is to create a Network architecture for an industry .which consists of so many member of employees with some rules and regulation the complete discription is mention in the PDF file
The SME should host three departments, Engineering, Sales and Management. The Engineering group will have, initially 300 computers, these are in turn divided into 200 staff computers and 50 build boxes (computers used to build and test solutions/products), 10 storage servers (where all the staffers store their data). The remaining 40 are production servers. These are deployed in groups of 5, i.e. 8 groups. Each group has two servers deployed in hot-swap load-balancing, the remaining three are used for service production. Using this basic production unit, the service can scale (add more prod units), and there is resilience since both load balancers as well as production are duplicated. The customer load is divided equally among the Prod servers, while the load balancers are run in hot-stand by. I.e. there is only one serving the customers, but if that fails, or needs to be shut down for maintenance the other takes over directl
The traffic patterns for the service groups are mentioned below . They are roughly equally loaded, except for group A and B. These are having roughly 10 times as many customers. Groups C—H have between 700 and 1200 customers/h. Service H is the beta-test for A, hence in not too long time, customers of A will move over to H, making the total customers in the 11-12K range.
Mbyte/customer

Mbyte/customer

Group

Customers/h

Load-In

Load-Out

A

10 000

0,01

1

B

10 000

0,02

2

C

1 000

5

10

D

900

7

2

E

730

0,001

1

F

100

5

10

G

1 000

10

0,001

H

1 200

0,02

4

The sales group consists of a back-office, of around 10 people; here 4 are technical writers working on documentation and adaptation of documentation, 4 are working as customer support (close cooperation with Engineering group and customers), the last 2 are sales people that work in the office. In addition to the back-office, the company has around 20 contracted sales people travelling the world (these are rotated back to the office once every few year).  The contacted sales people are responsible to buy their own laptops and peripherals, but they need to setup VPN connections to the main office to do their internal work. Hence, the network for the sales group has four different types of use; writing (4 computers), customer-support (4 computers), visiting-sales (30 computers, each sales person has a physical desktop in the office) and a VPN server (using a SPU deployment just as in production to ensure operations). The VPN traffic is moderate, at most 30 customers/h, however they generate around 10Mbps in/out traffic when they are active (using remote desktop). Once a remote sales person connects, they can start a remote desktop connection to their on-site desktop.

The management consists of a small team of five people; Chief Executive Officer (CEO), Technical Lead (TL, engineering manager), Sales Lead (SL, sales manager), Economic officer and a secretary. Each has a computer or two for (CEO, TL and SL).
In addition to this, there are some shared resources that cover all/some of the groups; 10 printers covering all groups, 2 file servers covering sales and management (Engineering has their own storage servers).

Within the nearest 6 months the company will:
Move customers from A to H service group, and rename H to A (basically update A). They anticipate a growth of customers of the updated A service, predicting to have 20000 customers/h 12 months after the update has launched (i.e. between 12 and18 months into the future, depending when the update occurs. They also anticipate the B service to grow, but to 15000 customers/h within the same time region.
Within 12 months:
The company will start beta tests of I and J services, these will run for 6 months, with around 1000 customers/h, like the current G and C services. When they launch, (x+6—12), they expect to have around 7000 customers/h.

The company also expects to grow the engineering group with 25-50 staff, sales with 5-6 contract sales people.

Within 24 months:
The company will expand with purchases of other groups, these will initially remain separate but during a 6-12 months period, their engineering groups will merge into the existing engineering group, however, they will not change location. Hence, the engineering group will be distributed, the same applies to for their services.

Propose a network design to match these requests. The design should include layer 2 and layer 3 devices and connectivity, and the required layer N infrastructure to support this.


