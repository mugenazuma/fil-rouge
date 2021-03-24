-- 2.1 - Elaborer le dictionnaire de données

-- A partir du cahier des charges, élaborez le dictionnaire des données :
-- Les descriptions devront être claires et réalistes.
-- Les informations devront être typées.


-- Product: 
* prod_id int(10) Primary Key
* prod_ref int(20),
* prod_name varchar(50),
* prod_desc varchar(255),
* prod_libel varchar(100),
* prod_price_ht decimal(10),
* prod_photo varchar(100),
* prod_stock_alert int(10),
* prod_quantity_stock int(10)
* prod_under_id int(10) Foreign key (sous_rubrique)

**********************

--  stock up  (approvisonnement)
* stock_id int(10) 
* stock_suppl_id int(10), Foreign key (fournisseur)
* stock_product_id int(10), Foreign key (produit) 
* stock_price_buying,
* stock_date_com date
* stock_date_livr date
* stock_qtite

**********************
-- clients
* cli_id int(10) Primary key
* cli_lastname varchar(50)
* cli_firstname varchar(50)
* cli_address varchar(255)
* cli_city varchar(10)
* cli_postcode char(15)
* cli_phone char(15)
* cli_mail varchar(50)
* cli_siret char(11)
* cli_commercial_id int(10) Foreign key (commerciaux)
* cli_type varchar(3) "par" pour particulier et "pro" déclenche la TVA ou non


**********************
-- commande
* com_id int(10) Primary key
* com_date date
* com_reduc
* com_price_tot
* com_date_regul
* com_date_facture
* com_deliv_adress
* com_deliv_city
* com_deliv_postcode char(15)
* com_facturation_address varchar(50)
* com_facturation_city varchar(50)
* com_facturation_postcode char(15)
* com_state varchar saisie, annulée, (en prépa, expédiée, facurée, retad de paiement, soldée)
* com_client_id int(10) Foreign key (client)

**********************
-- Commercial
* commer_id int(10) Primary key
* commer_lastname varchar(50)
* commer_firstname varchar(50)
* commer_tel
* commer_mail varchar(50) varchar(50)

**********************
-- contains
* cont_deliv_id int(10) Foreign key (livraison)
* cont_produt_id int(10) Foreign key (produit)

* cont_qtite_liv

*********************
-- supplier
* suppl_id int(10) Primary key
* suppl_name varchar(50)
* suppl_address varchar(100)
* suppl_postcod
* suppl_city varchar(50)
* suppl_phone char(15)
* suppl_lastname_contact
* suppl_firsname_contact

*********************
-- delivery
* deliv_id int(10) Primary key
* deliv_num_bon
* deliv_date date
* deliv_stat varchar(50) livrée, en cours , en prépa
* deliv_commande_id int(10) Foreign key (commande)

*********************
-- heading (rubrique)
* head_id int(10) Primary key
* head_name varchar(50)
* head_desc varchar(50)

********************
-- create of
* create_commande_id int(10) Foreign key (commande)
* create_produit_id int(10) Foreign key (produit)
* create_id int(10)
* create_order_price
* create_qtite_commande

********************
-- under heading (sous rubrique)
* under_id int(10) Primary key
* under_name varchar(50)
* under_desc varchar(100)
* under_head_id int(10) Foreign key (rubrique)

********************
-- followed
* follow_client_id int(10) Foreign key (client)
* follow_commer_id int(10) Foreign key (commerciaux)







