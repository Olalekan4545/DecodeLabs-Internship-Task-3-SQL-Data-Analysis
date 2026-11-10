Create Database Decodelabs 
Use [Decodelabs]
Select *
From [Decode Intenship ]


--- Question 1 : How many Orders are in the dataset
Select COUNT(distinct orderid) 'Total_Order'
From [Decode Intenship ]

-- the Total orders is 1,200


--- Question 2: what is the  total Recorded order value
Select SUM(Quantity) 'Total_Order_Value'
From [Decode Intenship ]



-- The total recorded order valuue is 3535

--- Question 3: what is Average order value
Select AVG(Quantity) 'Avg_Order_Value'
From [Decode Intenship ]

-- The average order value is 2

--- Question 4: which product have the highest order value
Select Top 1 Product,
SUM(Quantity) 'Total_order_Value'
From [Decode Intenship ]
Group by Product
Order by [Total_order_Value] Desc

--- Chair have the Highest order Value


--- Question 5: which payment method is used frequently 

Select Top 1 PaymentMethod,
COUNT(paymentmethod) 'Count_Payment'
From [Decode Intenship ]
Group by paymentmethod
order by [Count_Payment] Desc

--- The Payment Method Frequently used is "Online payment Method"


--Question 6 : What is the total Recorded value for each Payment Method
Select PaymentMethod,
Sum(TotalPrice) 'Total_Payment'
From [Decode Intenship ]
Group by paymentmethod


--- Question 7 : how many orders were cancelled

Select COUNT(orderstatus) 'Total Cancelled Order'
from [Decode Intenship ]
Where OrderStatus ='Cancelled'

--- the total cancelled order is 250

-- Question 8 : What is the total unit price for Each Product
Select Product,
Avg (UnitPrice) 'Average unit price'
From [Decode Intenship ]
Group by Product

--- Question 9 : Retrive orders where unit price is greater than 500, arranging the result from highesst to lowest 
Select OrderID, UnitPrice
From [Decode Intenship ]
Where UnitPrice >500
Order by UnitPrice Desc

--- Question 10 :how many orders was associated with each referral sources 
Select ReferralSource,
Count(OrderID) 'Total Orders'
From [Decode Intenship ]
Group by ReferralSource

-- Question 11: which coupon code Recorded the Highest order value

Select Top 1 Couponcode,
SUM(Quantity) 'Total Orders'
From [Decode Intenship ]
Group by Couponcode
