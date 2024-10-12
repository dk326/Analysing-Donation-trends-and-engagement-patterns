**About the Project**

The data for this project is from a non profit organisation. The purpose of this analysis was to understand the donation patterns across time and product type as well as engagement patterns of donors. Data was analysed using SQL on big query platform and Looker studio was used for visualisations. 

**Donation Trends**

By using a common table expression, 3 different tables are connected and data is retrieved for different metrics. Further, the donors are segmented into different age segments within this CTE. 

The main query selects the data from the CTE and other metrics. It also joins data from marketing campaign table where it exctracts year and month from the date column. Further, the final query filters out any null values. 

<img width="358" alt="Screenshot 2024-10-12 at 12 51 09 PM" src="https://github.com/user-attachments/assets/c937843e-7ecb-490e-812b-a86dd1eefced">

**Results*


<img width="1456" alt="Screenshot 2024-10-12 at 1 17 14 PM" src="https://github.com/user-attachments/assets/2bac145f-a8f2-4f52-b23f-a6dc7b16ccaf">

The resulting table from this query was imported to looker studio to create meaningful insights. 

**Insights*

**Donations by Year**

<img width="746" alt="Screenshot 2024-10-12 at 1 25 09 PM" src="https://github.com/user-attachments/assets/ca539786-2c51-466a-9f8a-a35504104c44">

- The total donation amount has been reduces in 2023 when compared with 2022.
- 
**Donations by year and Target Audience**

<img width="778" alt="Screenshot 2024-10-12 at 1 26 59 PM" src="https://github.com/user-attachments/assets/5b78521c-1ac2-4b02-ae3f-9984b9d75d27">

- When compared with 2022, in 2023 the gap between donations from new donors and other groups (High value and Returning) have been reduced.
- While the donation amounts from new donors have increased from $501725 to $ 686357, the donations from other two groups have been significantly reduced. ($1119300 to $818581 in high value and $1012078 to $655708 in returning donors)

**Donations by Month and Product type**

<img width="800" alt="image" src="https://github.com/user-attachments/assets/c3d1925f-be63-475d-8c2b-f074e53f6ac6">

- Insights into donation trends reveal variations based on product types.
- Donations peak significantly during the first five months of the year therefore, campaigns based on seasonality is recommended.
- The donation amount gap between memberships and other products is larger from January to May but becomes lower in the second half of the year.

**Monthly Donations by Campaign type**

<img width="800" alt="image" src="https://github.com/user-attachments/assets/debf3e54-34d3-49dd-805f-4f184f2a4af1">

- Donations from SMS campaigns peak in the first five months and decline significantly in the latter half of the year.
- Social media campaigns show a similar trend, with significant donations increasing from February to June; despite a decrease in the second half, they contribute more than other campaigns during this period.

**Monthly Donations by Audience type**

<img width="970" alt="Screenshot 2024-10-12 at 1 43 27 PM" src="https://github.com/user-attachments/assets/0423e904-763f-40f9-be5a-40a433c9c47d">

- The data reveals that donations from peak in the first half of the year with some fluctuations but deacreses in the second half.
- The Donations from new donors follow a similar pattern with increasing in the first half and reducing in the second half.
- However, the donations from returning donors does not decrease during the second half. However, there are fluctuations.
- All types of donors show an increase during the first half which could be an indication of seasonality or marketing efforts.

**Product Based Donations**

In this section, dontion amounts for different products by from donot segements have been analyzed. Further, the donations from these segements for marketing campaigns is also analyzed here. 

**Donation amount from each campaign type**

<img width="854" alt="Screenshot 2024-10-12 at 1 53 46 PM" src="https://github.com/user-attachments/assets/eef2da51-126a-4d6e-b8e8-dcba5a76da8e">

- The insights reveal that SMS and social media campaigns have been most effective as they have recieved donations of $ 1.5million each.
- Direct mail campaigns have been able to secure $1 million where as Email accounts for the lowest donations at $821K.

**Donation amount from each campaign type by year**

<img width="843" alt="Screenshot 2024-10-12 at 1 57 33 PM" src="https://github.com/user-attachments/assets/248c1035-4920-4453-aeb8-09ead923f305">

- It is important to note that in 2023 the donation amounts from Direct mail and Email campaigns have increased compared to 2022.
- Where as in the donations from SMS and Social media campaigns have been reduced significantly in 2023 than 2022.
- The reduction in donations from SMS and Social media campaigns is also reflected in the drop in total donations amount as visualised earlier. 
- However, the SMS and Social media accounts for the highest donations but the gap between donations from other campaigns have been narrowed.

**Average donation amount for different campaigns by customer age segments**

<img width="800" alt="image" src="https://github.com/user-attachments/assets/97a78569-3c9c-47ab-92d3-9e483dd2ddd8">

The analysis included patterns of past donations by campaign type and segmented donors into age categories:
- Children: Ages 7-14
- Young Adults: Ages 15-24
- Adults: Ages 25-44
- Established Adults: Ages 45-64
- Seniors: Ages 65-100
- Other ages labeled as unknown were excluded.

Key insights from the analysis include:

- Email campaigns are most effective for established adults and seniors, generating average donations of $264 and $249.90, respectively, but are least effective for children.
- SMS campaigns are highly effective for seniors, with an average donation of $304.50, and also work well for children at $280.20, but show low effectiveness for adults and young adults.
- Social media campaigns yield higher donations from seniors, established adults, and children, but are least effective for young adults.
- Direct mail campaigns are particularly effective for established adults, generating significant donations.

Average total donations by campaign type are:
- Email: $232.00
- SMS: $232.00
- Social Media: $227.00
- Direct Mail: $221.00

Total donations by campaign indicate SMS and social media are the most effective, with $1.5 million and $1.4 million, respectively, while direct mail generated $1 million and email $800,000.

**Average donation amount for different campaigns by customer age segments**

In order to identify donor engagement, the count of responses for an ad campaign was considered. Further, these were analyzed by different customer segments.

<img width="800" alt="image" src="https://github.com/user-attachments/assets/4678a087-36bd-4631-ad4f-8e25a886b385">

- The high-value donors have mostly responded to SMS marketing campaigns followed by email. They have responded least to direct mailing campaigns.
- Returning donors have mostly responded to social media marketing. They have equal responses for direct mail and SMS. Further, they are the least responsive for email campaigns.
- New donors have been mostly responsive to social media campaigns followed by SMS campaigns. They are also the least responsive for email campaigns. 


