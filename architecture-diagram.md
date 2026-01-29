# AWS VPC Architecture Diagram

```
                        Internet
                            |
                     +----------------+
                     | Internet Gateway|
                     +----------------+
                            |
                -----------------------------
                |                           |
        Public Route Table           Private Route Table
        0.0.0.0/0 → IGW              0.0.0.0/0 → NAT GW
                |                           |
        -------------------        -------------------
        |  Public Subnet   |        | Private Subnet  |
        | 10.0.0.0/24      |        | 10.0.1.0/24     |
        |                  |        |                 |
        |  EC2 (Public)    |        |  EC2 (Private)  |
        |  Public IP       |        |  No Public IP   |
        -------------------        -------------------
                |
        -------------------
        | NAT Gateway     |
        | Elastic IP      |
        -------------------
```

## Key Points

- IGW provides internet access to public subnet
- NAT Gateway allows outbound access for private subnet
- Private subnet is fully isolated from inbound internet traffic
