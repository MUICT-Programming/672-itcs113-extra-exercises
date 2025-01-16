## Hotel Booking Discounts Exercise

Customer: Ask if the customer is a "Regular" or "First-time" guest.

Regular Guest:

- Continue to ask how many nights the guest is booking.
  - If the number of nights is more than 5, offer a 15% discount.
  - Otherwise, offer a 10% discount.

First-time Guest:

- Ask if they are booking a "Single" or "Double" room.
  - Single room: No discount.
  - Double room: Offer a 5% discount.
 
## Cinema Ticket Pricing Exercise

Customer: Ask the customer for their age group: **"Child," "Adult," or "Senior."**

Child (age < 12):

- Ask if they want snacks (Yes/No).
  - Yes: Offer a 5% discount on snacks.
  - No: Offer a 10% discount on the ticket price.

Adult (age 12–59):

- Ask if they are watching during **"Weekday" or "Weekend."**
  - Weekday: Offer a 10% discount on the ticket price.
  - Weekend: No discount on the ticket price but offer free popcorn.

Senior (age ≥ 60):

- Ask if they are coming **alone or with family.**
  - Alone: Offer a 15% discount on the ticket price.
  - With family: Offer a 20% discount for the entire group.

## Restaurant Dining Discounts Exercise

Customer: Ask if the customer is dining "Alone," "With Family," or "With Friends."

Alone:

- Ask if they are ordering from the "Set Menu" or "À la Carte."
  - Set Menu: Offer a 5% discount.
  - À la Carte: No discount.

With Family:

- Ask if the family has children under 12.
  - Yes: Offer a 10% discount on the total bill.
  - No: Offer a free dessert for everyone.

With Friends:

- Ask if the group size is larger than 4 people.
  - Yes: Offer a 15% discount on the total bill.
  - No: No discount but include a free appetizer.

## Tax Calculation Exercise

Customer: Provide the customer's **total income** to calculate the tax based on the following criteria.

### For Individuals:
- If the total income is **$0–$50,000**, apply a **10% tax rate**.
- If the total income is **$50,001–$100,000**, apply a **20% tax rate**.
- If the total income is **above $100,000**, apply:
  - A base tax of **20%** on the first $100,000.
  - An additional **5% surcharge** on the amount exceeding $100,000.

### For Businesses:
- If the business is classified as a **Small Business**:
  - If the total income is **$0–$250,000**, apply a **15% tax rate**.
  - If the total income is **above $250,000**, apply:
    - A base tax of **15%** on the first $250,000.
    - A **25% tax rate** on the amount exceeding $250,000.
- If the business is classified as a **Corporation**:
  - Apply a **30% tax rate** on the total income.
  - If the business employs **more than 50 employees**, apply an additional **2% workforce tax** on the total income.


## Test Cases

### Test Case 1: Individual, Income Below $50,000

Input:
```
I 40000
```
Expected Output:
```
TaxRate 10
TaxAmount 4000
```

### Test Case 2: Individual, Income Between $50,001 and $100,000
Input:
```
I 75000
```
Expected Output:
```
TaxRate 20
TaxAmount 15000
```

### Test Case 3: Individual, Income Above $100,000
Input:
```
I 150000
```
Expected Output:
```
TaxRate 22500
TaxAmount 22500
```

### Test Case 4: Small Business, Income Below $250,000
Input:
```
B 200000
```
Expected Output:
```
TaxRate 15
TaxAmount 30000
```

### Test Case 5: Small Business, Income Above $250,000
Input:
```
B 300000
```
Expected Output:
```
TaxRate 50000
TaxAmount 50000
```
### Test Case 6: Corporation, No Additional Workforce Tax
Input:
```
C 500000 40
```
Expected Output:
```
TaxRate 30
TaxAmount 150000
```

### Test Case 7: Corporation, With Additional Workforce Tax
Input:
```
C 500000 60
```
Expected Output:
```
TaxRate 32
TaxAmount 160000
```

**Important: these questions are ChatGPT generated.**
