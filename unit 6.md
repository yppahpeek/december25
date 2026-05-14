# DevOps Unit 6: Collaboration & Data Processing

## Part 1: Remote Version Control Setup
- ☑️ Create a new private repository on GitHub without adding a README or .gitignore file .
-  ☑️ Link the local repository to the remote origin using `git remote add origin https://...` .
-  ☑️ Push the local `main` branch to GitHub using `git push -u origin main` .
-  ☑️ Checkout the `read_csv` branch and push it to GitHub using `git push origin read_csv` .
-  ☑️ Create a Pull Request (PR) on GitHub to merge the `read_csv` branch into the `main` branch .
-  ☑️ Merge the PR to incorporate the changes into the main branch .
-  ☑️ Checkout the local `main` branch and pull the changes manually using `git pull origin main` .

## Part 2: Feature Development (TDD Cycle)
**Feature 1: Match Data**
  -  ☑️ Checkout a new branch named `match_data` .
  -  ☑️ Write a failing test for merging stock and sales datasets by `product_id` .
  -  ☑️ Implement `merge_data` to make the test pass .
  -  ☑️ Create the `src/main.py` entrypoint and manually test the execution .
  -  ☑️ Commit, push, create a PR, and merge into `main`.

**Feature 2: Subtract Values & Update Dates**
  -  ☑️ Write a test and implement `update_stock` to subtract sales from the stock data .
  -  ☑️ Refactor tests to use a `@pytest.fixture` to supply the merged data .
  -  ☑️ Modify `update_stock` to update the `last_stock_update` date based on the sales data.

**Feature 3: Output Processed Data**
  -  ☑️ Write a test and implement `write_data` to output the processed data as a CSV .
-  ☑️ **Feature 4: Low Stock Reporting**
  -  ☑️ Checkout a new branch called `write_reorder_file` .
  -  ☑️ Write a test and implement `get_low_stock_products` and `write_reorder_file` .
  -  ☑️ Merge the changes back into the `write_csv` branch, and then merge into `main` .
  -  Andy Test for pull request
