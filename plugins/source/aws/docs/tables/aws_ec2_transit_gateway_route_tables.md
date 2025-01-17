# Table: aws_ec2_transit_gateway_route_tables

This table shows data for Amazon Elastic Compute Cloud (EC2) Transit Gateway Route Tables.

https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_TransitGatewayRouteTable.html

The composite primary key for this table is (**account_id**, **region**, **transit_gateway_arn**, **id**).

## Relations

This table depends on [aws_ec2_transit_gateways](aws_ec2_transit_gateways.md).

## Columns

| Name          | Type          |
| ------------- | ------------- |
|_cq_id|`uuid`|
|_cq_parent_id|`uuid`|
|account_id (PK)|`utf8`|
|region (PK)|`utf8`|
|transit_gateway_arn (PK)|`utf8`|
|id (PK)|`utf8`|
|creation_time|`timestamp[us, tz=UTC]`|
|default_association_route_table|`bool`|
|default_propagation_route_table|`bool`|
|state|`utf8`|
|tags|`json`|
|transit_gateway_id|`utf8`|
|transit_gateway_route_table_id|`utf8`|