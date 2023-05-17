## Jaffle Shop & Stripe - Ready Analytics

Jaffle_shop is a fictional ecommerce store and Stripe is an online payment gateway.
A fundamental dbt project is built that transforms raw data from the app database into a model ready for analytics.

### Stack :
    Source : Jaffle_shop & Stripe (Data from S3)
    Data Platform : Snowflake
    Tranformation tool : Dbt
    Target load : Snowflake
    Scheduled within Dbt

### Running the workflow 

    Install dbt 
    Clone this repository.
    Change into the jaffle_shop directory from the command line:
    $ cd jaffle_shop
    Create an account in any of the data platforms (snowflake / big-query / local postgres database)
    Connect the dbt profile to the data warehouse (Snowflake in this scenario)
    Run the source_load.sql file to load data to the data warehouse (mock-up)
    Use the following commands to run the project in CLI :
        $ dbt debug
        $ dbt seed
        $ dbt run
    Test the output of the models:
      $ dbt test
    Generate documentation for the project:
      $ dbt docs generate
    View the documentation for the project:
      $ dbt docs serve
    Schedule the job in a different environment (deploy) and test the same
