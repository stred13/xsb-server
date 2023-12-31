# xsb-server

1. **Title** : XSB
2. **Description:**

XSB is a user-friendly mobile application designed to simplify the process of splitting group bills among friends, roommates, or colleagues. With intuitive features and a clean interface, users can effortlessly create, manage, and settle bills within their groups. The application focuses on transparency, ease of use, and accurate expense calculations to ensure fairness in every financial transaction.

3. **Objectives:**

- **Simplicity** : Users can easily to input expenses and share bills to participants effortlessly.
- **Accessibility** : Create a cross platform application. Able to access web or mobile.
- **Transparency** : User can have detail logs to track expenses.

4. **Functional features:**

4.1. **Expense input:**

- Add new bills with details of expenses (title, description, amount)
- Input individual expenses and add participants to share bills.

4.2. **Calculation** :

- Calculate the amount for each participant base on input expenses.
- Handle many types of splitting bills (equal, percentage, itemized)

4.3. **Display expenses in detail:**

- Display a detail of each expense and each participants' contribution.

4.4. **Logs:**

- Add, Edit, or delete bills and participants.

4.5. **Notifications:**

- Notification if any changes (add/edit/delete)

5. **Non-functional features:**

- **Security** : Implement secure authentication and authorization.
- **Scalability** : Handle a growing number of users and transactions.
- **Performance** : Quick, and immediately response data/calculation/notification.
- **Cross platform** : Application for web and mobile platforms.
- **Outage** : Able to input expenses even outage.

6. **User stories:**

- As a User, I want to create a new bill entry with details of expenses and participants.
- As a User, I want to input individual expenses and specify who participated in each expense.
- As a User, I want the application to calculate each participant's share based on the expenses and participants involved.
- As a User, I want to view a detailed breakdown of expenses and each participant's contribution.
- As a User, I want to save and retrieve bill histories for future reference or recurring bills.
- As a User, I want the option to edit or delete bill entries and participants.
- As a User, I want to receive notifications or summaries of shared expenses.
- As a User, I want to login to application to track and manage expenses.
- As a User, I want to add new participants to a group for share bills.
- As a User, I want to join a group for share bills using a code, or QR code.
- As a User, I want to search for group share bills by title.
- As a User, I want to sort group bills with the latest on top.

7. **Key Features:**
7.1. **User Registration and Group Creation:**

- Users can create accounts and set up groups for various occasions or shared expenses.
- Users also login via Google, Facebook.
- Invite friends to join the group using short link. Such as: [xsb.com/mysharebill](http://xsb.com/mysharebill).

  **In details:**

    - Users can register using email or Single Sign-On (SSO) with Facebook or Google. Anonymous users can continue using the application without creating an account.
    - Only registered users can create a new X Share Bill, while anonymous users can join existing XSB groups.
    - Group members can view history and expenses.
    - Profile management for registered accounts includes nickname, email, and profile picture.

7.2. **Create a New XSB group and Add people to XSB group:**

- Users can easily create a new XSB group, specifying details such as the title, description of the expense, currency, and category.

  **In details:**

  - Users can create a new XBS groups, like "Trip to Dallas", "Journey to Mekong Delta River".
  - Participants can be added to the XSB group with a display name (e.g., Participants: Kim, Triet, Nam). Optional: Email
  - Users can create shorten link and share to social media. Such as: [xsb.com/mysharebill](http://xsb.com/mysharebill).
  - A QR code can be generated for easy group joining.

7.3. **Expense Editing and Deletion in XSB group:**

- Users can add/edit the details of a bill, such as the title, amount, date, paid by, share money for whom, attach photo as a receipt, add a category.
- Delete bills if a transaction was added by mistake or is no longer relevant.

  **In details:**

    - Users can add a new bill or edit details to correct data such as title, amount, date, paid by, share money for whom.
    - Photo attachments can be taken for the current receipt.
    - Existing attachments in the list can be deleted.

7.4. **Real-time Expense Calculation:**

- The application automatically calculates each participant's share based on their contributions.
- Users can view real-time updates on who owes or is owed money within the group.

  **In details:**

- Equal split: The bill will be divided equally among all participants.
  Formula: Equal Share = Total Bill Amount / Number of Participants.

- Itemized split: Users can assign specific items to individuals. Participants not joined in the bill are excluded from the list.
  Formula: Share for each participant = Total cost of items assigned to the participant.

- Rounded calculation: Bills are rounded up for clarity.
  Formula: Rounded Share = Round(Share for each participant).

- Advanced: In an XSB Bill, many people can join to pay, but not all contribute equally. Bills must be separated and then shared among all participants.

7.5. **Expense History and Reports: X Balance Tab**

- Generate reports summarizing expenses, including individual contributions and balances.

  **In details: X Balance Overview**

  - The X Balance Tab provides users with a comprehensive overview of all outstanding balances within the group.
  - It displays a list of participants, highlighting who owes money (negative balance) and who is owed money (positive balance).
  - Reimbursement: Automatic suggestion for reimbursing participants base on the expenses they've covered for the XSB group.
  - Marked as paid.

  - **Recent activity:**

    - You updated "Rent a bike" in "Trip to Dallas" - Amount: $ 50.00
    - Tred added "Hotel" in "Trip to Dallas" - Amount: $10.00
    - NAM NGUYEN HOANG added an expense: Rent a car ($5,000)
    - NAM NGUYEN HOANG added a member: LE NGUYEN

8. **Notifications:**

- Send notifications to group members via mails.

9. **Security and Privacy:**

- **Security: Assigned to Triet and Kim**
- **Privacy: Assigned to Nam.**

10. **Multi-platform Support:**

- Develop the application for Web applications. Responsive must be applied.
- Develop the application for both iOS and Android platforms.

11. **Export and import:**
12. **Search feature.**