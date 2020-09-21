# Appendix 3 Filter Criteria Description

**What are filter criteria?**

If you have read the content of Appendix 2 Journey Controls Description, then you must have an impression of the judgment controls such as Event condition, Variable condition and Condition split. The filter criteria is the judgment symbol. For example, the gender of the contact is equal to male, and equal to is the filter criteria.

The filtering criteria can be divided into three types according to the data type: 

1\)String type

![](.gitbook/assets/image%20%28550%29.png)

![](.gitbook/assets/image%20%28547%29.png)

### Belong Description 

Example: The creation form contains the field named Product Category, which includes shoes, clothes and snacks. Shoes include leather shoes, sports shoes and high heels. Clothes include suits, dresses and underwear, and snacks include instant noodles, candy and jelly.

![](.gitbook/assets/image%20%28527%29.png)

After collecting the user statistics, we need to filter out the users who choose any one of sports shoes, leather shoes, high heels, suits, dresses and underwear. At this time, we can use the belong operator, which indicates that the value is equal to any value within the specified values.

![](.gitbook/assets/image%20%28565%29.png)

As the figure show above, we could set the filter criterion as Product Category belongs to shoes and clothes, which indicates the value selected by the user in the Product Category field is one of shoes or clothes. That is, the value selected by the user is one of sports shoes, leather shoes, high heels, suits, dresses and underwear. 

2\)Numerical type \(integer and decimal\)

![](.gitbook/assets/image%20%28510%29.png)

![](.gitbook/assets/image%20%28573%29.png)

3\)Time type

![](.gitbook/assets/image%20%28541%29.png)

![](.gitbook/assets/image%20%28500%29.png)

