# googleinfringements

As of 1. June 2016

               Table "public.domains"
    Column    |          Type           | Modifiers
--------------+-------------------------+-----------
 requestid    | integer                 |
 domain       | character varying(3000) |
 urlsremoved  | integer                 |
 urlsnoaction | integer                 |
 urlspending  | integer                 |
 fromabuser   | boolean                 |

TOTAL number of rows: 107'414'172

                          Table "public.requests"
              Column              |            Type             | Modifiers
----------------------------------+-----------------------------+-----------
 request_id                       | integer                     |
 date                             | timestamp without time zone |
 lumen_url                        | character varying(1000)     |
 copyright_owner_id               | integer                     |
 copyright_owner_name             | character varying(1000)     |
 reporting_organization_id        | integer                     |
 reporting_organization_name      | character varying(1000)     |
 urls_removed                     | integer                     |
 urls_for_which_we_took_no_action | integer                     |
 urls_pending_review              | integer                     |
 from_abuser                      | boolean                     |

TOTAL number of rows: 3'505'553

        Table "public.urls_no_action_taken"
   Column    |           Type           | Modifiers
-------------+--------------------------+-----------
 request_id  | integer                  |
 domain      | character varying(2000)  |
 url         | character varying(15000) |
 from_abuser | boolean                  |

TOTAL number of rows: 40'188'142
