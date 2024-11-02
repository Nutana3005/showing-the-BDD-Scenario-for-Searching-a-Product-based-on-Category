# showing-the-BDD-Scenario-for-Searching-a-Product-based-on-Category
Scenario: Searching products by category
  Given the following products
    | name      | category | available |
    | ToyCar    | Toys     | true      |
    | BoardGame | Games    | true      |
  When I search for products in category "Toys"
  Then I should see 1 product with category "Toys"
