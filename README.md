# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

==> The Depot Online Store
 
This application implements an online store, with a catalog, cart, and orders.
 
It is divided into two main sections:
 
* The buyer's side of the application manages the catalog, cart, 
  and checkout. It is implementation spans in four models and associated
  controllers and views: Cart, LineItem, Order, and Product.  Additionally,
  there is a StoreController for the store front itself, and a
  SessionsController to manage sessions.
 
* Only administrators can access stuff in the seller's side
  (product maintenance and order fulfillment).  This is implemented by the
  SessionsController, is enforced by the ApplicationController#authorize
  method, and assisted by the Users and Carts resources.
 
=== Authors
 
 * Sam Ruby, IBM
 * Dave Thomas, The Pragmatic Programmers, LLC
 * David Heinemeier Hansson, 37signals
 
