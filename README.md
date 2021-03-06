# Yelp-Review-Search

It is a standalone application which runs queries on the Yelp data and extracts useful information. The
primary users for this application will be potential customers seeking for businesses and users that match their
search criteria. This has a user interface that provides the user the available business categories
(main, sub-categories), the attributes associated with each business category along with business review and yelp
user information associated with each business category. Using this application the user will search for the
businesses from various business categories that have the properties (attributes) the user is looking for. 

![alt text](https://github.com/pratiksaha37/Yelp-User-Search/blob/master/Yelp%20Review%20Search.JPG)

# Business Search: A GUI where the user can search for movies that match the criteria given.
o Browse through main categories for the businesses (See Appendix C); select the business
attributes that user wants to search for;
**note:** The list of the main categories is given in Appendix-C. All other categories that appear in the
business objects are sub-categories. Such a distinction is made for easier browsing of the business
categories.

# The usage flow of the GUI is as follows:
1) Once the application is loaded, main categories are loaded from the backend database. 
**Note that**, selection of business main categories (single or multiple) is required. For instance, assume
that use selects Restaurants as the main category.
2) The subcategories matching the main category selection will be listed under subcategories
column. Since user selected Restaurants in previous step, only sub-categories values that its
main category is Restaurants should appear in the sub-categories panel. Note how faceted
search work here. After step 1, the set of results is reduced to only the businesses that belong to
Restaurants category. The user can select desired sub-categories values. This attribute is
optional in building the query. User might not select a sub-category at all. Assume that use
selects Mediterranean as the sub-category value.
3) Attribute column is the next selection. Similar to No 2, the set of results is reduced to only the
subcategories AND main category selection. The user can select desired attribute values (single
or multiple selections). This attribute is optional in building the query. User might not select a
attribute values at all. Since user selected Restaurants, and Mediterranean in previous steps, 
3
only attribute values that appeared in business with main-category = Restaurants AND subcategory
= Mediterranean, should appear in the attribute selection panel. Assume that user
selects Outdoor Sitting as the desired attribute.
4) Review column is the next selection. You can specify review duration (from/to) and enter the
star and vote values into the text box. The attributes under the Review column are also optional.


![alt text](https://github.com/pratiksaha37/Yelp-User-Search/blob/master/Business%20Query.JPG)


# User Search:  The usage flow of the GUI is as follows:
1) User can specify user search using attributes such as member_since, review_count, number of
friends, verage stars and number of friends.
2) Clicking on “Execute User Query” will show user matches, yelping_since and average_stars
3) select a certain user in the search results and list all the reviews given by that user.
**Note:** The user can do either a Business search or User search (not both) at any given time through the GUI.
**Note:** All data displayed on the GUI should be kept in the database and should be retrieved from it when needed.
You are not allowed to create internal data structures to store data.

![alt text](https://github.com/pratiksaha37/Yelp-User-Search/blob/master/User%20Search.JPG)
