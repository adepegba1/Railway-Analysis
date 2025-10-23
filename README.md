# 🚆 Railway Ticket Sales & Delay Analysis

## 📘 Introduction
This project analyzes data from a railway ticketing system to uncover insights into customer purchasing behavior, route popularity, ticket pricing trends, and journey delays. Using Python (Pandas, Matplotlib, and Seaborn), the analysis explores patterns that can inform business decisions and improve operational efficiency.

- The key objectives of this project were:

  - To identify top-performing routes and revenue sources.  
  - To evaluate purchasing behavior (online vs station sales).  
  - To analyze delay causes and their relationship to refunds.  
  - To understand ticket price variations by class and type.  
  - To discover time- and season-based trends in sales and delays.

## ⚙️ Methodology
### Data Source
The dataset (railway_new.csv) contains records of railway ticket transactions, including:

- Transaction ID, Date & Time of Purchase
- Purchase Type (Online / Station)
- Payment Method
- Ticket Class (Standard / First)
- Ticket Type (Advance, Anytime, Off-Peak)
- Journey Status (On Time / Delayed)
- Reason for Delay
- Refund Requests
- Price

### Data Cleaning

- Standardized categorical values (e.g., unified “Signal failure” → “Signal Failure”).
- Removed duplicate rows (none found).
- Converted date and time columns to datetime format.
- Created derived columns for Month, Time of Day, and Weekday/Weekend for trend analysis.

### Tools Used

- **Python Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook
- **Visualization:** Bar charts, pie charts, tables

## 📊 Findings
### Revenue Insights
- Total revenue generated: $741,921
- Highest revenue month: January ($205,091)
- ✔ Suggests strong seasonal or holiday demand.

### Customer Purchase Behavior
- Most popular purchase type: Online (18,521 sales)
- ✔ Reflects growing preference for digital ticketing.

- Most frequent purchase time: Morning (16,160 purchases)
- ✔ Customers tend to plan or book early in the day.

### Popular Routes
Top 5 routes by ticket sales volume:
<table>
  <thead>
    <tr>
      <th>Departure Station</th>
      <th>Arrival Destination</th>
      <th>Sales</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Manchester Piccadilly</td>
      <td>Liverpool Lime Street</td>
      <td>4,628</td>
    </tr>
    <tr>
      <td>London Euston</td>
      <td>Birmingham New Street</td>
      <td>4,209</td>
    </tr>
    <tr>
      <td>London Kings</td>
      <td>Cross	York</td>
      <td>3,922</td>
    </tr>
    <tr>
      <td>London Paddington</td>
      <td>Reading</td>
      <td>3,873</td>
    </tr>
    <tr>
      <td>London St Pancras</td>
      <td>Birmingham New Street</td>
      <td>3,471</td>
    </tr>
  </tbody>
</table>		
		
### Ticket Pricing
<table>
  <thead>
    <tr>
      <th>Ticket Class</th>
      <th>Avg. Price</th>
    </tr> 
  </thead>
 <tbody>
  <tr>
    <td>Standard</td>
    <td>$20.72</td>
  </tr>
  <tr>
    <td>First Class</td>
     <td>$48.86</td>
  </tr>
 </tbody>
</table>


Ticket Type Impact:

Type	Avg. Price
Advance	$17.61
Off-Peak	$25.52
Anytime	$39.20

➤ Advance tickets are cheaper, encouraging early bookings.

5. Delay Analysis

Delayed vs On-time journeys:
Pie chart shows ~27% delays vs 73% on-time.

Most delayed route:
Liverpool Lime Street → London Euston (780 delays)

Top reasons for delay:

Signal Failure

Bad Weather

Technical Faults

Congestion

Staff Shortage

6. Refund Behavior

Refunds from delayed journeys: 546 cases

23.8% of refunds were due to delays.

Refunds more common at stations than online — possibly due to ease of in-person claims.

7. Weekend vs Weekday Performance
Period	Delayed Journeys
Weekdays	1,642
Weekends	650

➤ More delays occur during weekdays, likely due to heavier commuter traffic.

💡 Recommendations

Improve Route Reliability:

Prioritize maintenance on Liverpool–London and Manchester–Liverpool routes.

Invest in signal infrastructure to address the leading cause of delays.

Enhance Online Refund System:

Simplify digital refund requests to match the convenience of station-based claims.

Promote Off-Peak and Advance Sales:

Offer discounts or loyalty points to shift demand away from peak hours.

Dynamic Pricing Strategies:

Adjust ticket prices based on seasonality and purchase time (morning vs afternoon).

Customer Communication:

Use purchase time and route data to send real-time notifications and travel updates.

🧭 Conclusion

This analysis highlights that:

Online purchases dominate the market.

Weekday congestion and signal failures are major delay drivers.

Advance tickets attract price-sensitive travelers, while first-class tickets yield higher per-ticket revenue.

Improving infrastructure and refund systems can enhance customer satisfaction and revenue retention.

Overall, the insights enable data-driven decision-making in operations, pricing, and customer engagement strategies.
