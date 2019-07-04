# bank-kata-bootstrap
Bootstrap for TDD bank kata (or any kata, really)


Kata: a Japanese word, meaning literally: "form" (型 or 形):
“a detailed choreographed pattern of movements made to be practiced alone, but are also practiced within groups and in unison when training.”


## Problem Description
- Deposit into the Account
- Withdraw from the Account
- Withdraw from the Account

Statement should have following format: 

```
> DATE       | AMOUNT  | BALANCE
> 10/04/2019 | 100.00  | 900.00
> 09/04/2019 | -200.00 | 800.00
> 01/01/2019 | 1000.00 | 1000.00
```

## Constraints
1. Start with class with follwing structure:
```
Public class Account {
   public void deposit(int amount) {}
   public void withdraw(int amount) {}
   public void printStatement() {}
}

```

2. You are not allowed to add/change any other public methods or public fields to the class – apart from a constructor

3. Use strings and integers for dates and amounts (keep it simple)

4. Don’t worry about spacing in the printed statements


## TDD Constraints

1. You are not allowed to write a single line of implementation code unless there’s a test for it

2. If you think of an edge case, make a test, then go back and refactor till it works.


## Tips
- Think -> Test -> Implement
- Red -> Green -> Refactor -> GOTO Red
- Wrap IO calls with your own Console that you can stub and verify against 
- Your Account will probably need a Ledger, containing all the Transactions
- Use your testing library of choice; Mockito and Assert4J is probably the java weapon of choice for this.

- If you feel _really_ confident, start by writing an acceptance test against the Account

