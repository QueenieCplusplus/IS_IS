# IS_IS
relative to OSPF

IS-IS is ISO Dynamic Routing Spec, it is a link-state routing protocol that floods link-state info building topology thru network.

It can route IP packets and route CNLP, conectionless network protocol packets. IS-IS is deemed to be an alternative to OSPF and EIGRP.

It is commonly used in ISP network, but merely to be seen in Enterprise network.

# Definition of Metrics

It uses a metric wiht a max path value of 1024. It is intended to measure the capacity of circuit of traffic, such as it thruput in bps.

              Higer Value indicates Lower Capacity.
              
Any single link can have a max value of 64. IS-IS calculates path values by sum up links values. In this way, it helps to check the shortest-path algorithm is executed effectively and its metrics provide the granularity to support diversified link types.

# Apply to Cisco Router

Their interface's default metric is 10. Thus Administrator shall config the value.

           Small Value proofs insufficient to Large Network(High Bandwidth)

This is whay Cisco uses "wide metrics" instead now.
