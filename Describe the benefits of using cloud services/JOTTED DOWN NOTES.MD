# Benefits of High Availability and Scalability in the Cloud

Two biggest consideration when building a cloud application is the uptime (availability) and the ability to handle demand (or scale).

## High Availability
- Ensures IT resources and applications are available when needed.
- Focuses on maintaining uptime despite disruptions.
- Azure offers service availability guarantees through **Service Level Agreements (SLAs)**.

Azure SLA are represented as a percentage related to applications or services' availability. This availability is also known as uptime. If the service was always available to use, you'd say it was 100% available or it had 100% uptime.
- SLA commonly includes details like what is defined as down time, when the service is unavailable, and any credit you may be entitled to if the SLA is not met. 

In reality, 100% uptime is difficult and expensive to achieve. Bceause it will require duplicating every single component in case one component failed and would require those backup components to pick up the service tasks with zero interruption to the customer.

Is there a difference in 99% vs 99.9% SLA? Yes! 

- A service with a 99% SLA percentage can be unavailable for up to 1.6 hours per week 0r 7.2 hours per month, and still be 99& available.

- A service with the 99.9 SLA percentage can be unavailable for only 10 minutes per week or 43.2 minutes per month.

**EACH AZURE SERVICE HAS ITS OWN SLA. FAMILIARIZE YOURSELF WITH THEM.

## Scalability
- Adjusts cloud resources to meet demand efficiently.
- Helps prevent system overloads during peak traffic.
- Reduces costs by scaling down unused resources.
- Operates on a **consumption-based pricing model**—pay only for what you use.

### Types of Scaling:
#### Vertical Scaling:
- Increases or decreases resource capabilities (CPU, RAM).
- Example: Upgrading or downgrading a virtual machine's specs.

#### Horizontal Scaling:
- Adjusts the number of deployed resources dynamically.
- Example: Adding or removing virtual machines or containers based on demand.

By leveraging **high availability** and **scalability**, cloud solutions can maintain uptime and optimize costs effectively.
