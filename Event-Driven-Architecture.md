# [AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

## When to use SNS or SQS

**SNS** - sends **messages** to the **subscriber** using **push** mechanism and no need of pull.

**SQS** - a message **queue service** used by distributed applications to **exchange** messages through a polling model, and can be used to **decouple** sending and receiving components.

These services provide different benefits for developers. Amazon **SNS** allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates.

How do you use SNS with SQS?
1. On the **Create** subscription page, in the Details section, do the following:
1. For Topic ARN, enter the ARN of the topic.
1. For Protocol, choose Amazon SQS.
1. For Endpoint, enter the ARN of the queue.
1. Choose Create subscription. 