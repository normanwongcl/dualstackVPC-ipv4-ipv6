# Dualstack IPv4/IPv6 VPC network (Discontinued)

This repository provides a set of YAML templates to create a dualstack IPv4 and IPv6 VPC in AWS.

## Goals
- The aim of this project was to build out an over-complicated IPv4/IPv6 network in AWS from scratch during my free time.
- To be used as future reference material for myself.


## Overview

![infrastructure-overview](images/overview.png)

### Categories

- [VPC](#vpc)
- [Security Groups](#security-groups)
- [NACL](#nacl)
- [Endpoints](#endpoints)

## Templates

[Back to Top](#overview)

### VPC

[Back to Top](#overview)

<table width="100%">
    <tr>
        <th align="left" colspan="2"><h4><a href="https://github.com/Klezca/dualstackVPC-ipv4-ipv6/blob/master/templates/vpc.yaml">VPC</a></h4></th>
    </tr>
    <tr>
        <td width="100%" valign="top">
            <p>Select the foundational pieces for building out a dualstack IPv4/IPv6 VPC network from the ground up.</p>
            <h6>Create Details</h6>
            <ol>
                <li>VPC</li>
                <li>VPC Flow Log</li>
                <li>IPv6 Cidr Block</li>
                <li>Internet Gateway</li>
                <li>Egress Internet Gateway</li>
                <li>3 NAT Gateways</li>
                <li>3 Public Subnets</li>
                <li>3 Public-NAT tier Subnets</li>
                <li>3 Private Web-app tier Subnets</li>
                <li>3 Private MySQL-RDS tier Subnets</li>
                <li>3 Private Redis-Elasticache tier Subnets</li>
                <li>Route Tables</li>
                <li>IPv6 workaround IAM role and Lambda with python runtime</li> 
            </ol>
        </td>
        <td  nowrap width="200" valign="top">
            <table>
                <tr>
                    <th align="left">View Diagram</th>
                </tr>
                <tr>
                    <td>
                        <a href="images/diagrams/vpc.png" target="_blank"><img src="images/diagrams/vpc.png" width:100% alt="View Diagram"></a>
                    </td>
                </tr>
            </table>
        </td>
    </tr>
</table>

### Security-Groups

[Back to Top](#overview)

<table width="100%">
    <tr>
        <th align="left" colspan="2"><h4><a href="https://github.com/Klezca/dualstackVPC-ipv4-ipv6/blob/master/templates/security-groups.yaml">Security Groups</a></h4></th>
    </tr>
    <tr>
        <td width="100%" valign="top">
            <p>Select the foundational pieces for building out the necessary security groups.</p>
            <h6>Create Details</h6>
            <ol>
                <li>Web Server Security Group</li>
                <li>Load Balancer Security Group</li>
                <li>MySQL RDS Security Group</li>
                <li>Redis Elasticache Security Group</li>
                <li>VPC Endpoints Interface Security Group</li>
                <li>ICMPv4 and ICMPv6 Security Group (optional)</li>
            </ol>
        </td>
        <td  nowrap width="200" valign="top">
            <table>
                <tr>
                    <th align="left">View Diagram</th>
                </tr>
                <tr>
                    <td>
                        <a href="images/diagrams/security-groups.png" target="_blank"><img src="images/diagrams/security-groups.png" width:100% alt="View Diagram"></a>
                    </td>
                </tr>
            </table>
        </td>
    </tr>
</table>

# Work in Progress
