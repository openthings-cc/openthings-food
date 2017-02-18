# openthings-food

Food mappings playground

This is an experimental repo which aims to create mappings and common ontology to describe:

* food items
* food products
* food producers/farmers
* delivery chain and actors
* food shops/hubs
* collaboration between those

the result of this effort may eventually be stored and maintained in the central repo for openthings.cc ontologies - https://github.com/openthings-cc/openthings-onto

## Similar:

* https://aims-fao.atlassian.net/wiki/display/AGV/Releases (http://aims.fao.org/vest-registry/vocabularies/agrovoc-multilingual-agricultural-thesaurus)
* https://circabc.europa.eu/faces/jsp/extension/wai/navigation/container.jsp
* http://data.lirmm.fr/ontologies/food#
* http://www.w3.org/TR/2004/REC-owl-guide-20040210/food.rdf (demo)
* https://raw.githubusercontent.com/ailabitmo/food-ontology/master/food.owl (https://fruct.org/publications/abstract13/files/Kol.pdf)
* http://semanticdiet.com/data.event (some research around USDA)


## Analysis

* (food1) http://data.lirmm.fr/ontologies/food#

Used in Open Food Facts(OFF) LOD. It defines basic classes for Food product and detailed ingredient properties.
It is simple and practical.. for generic food product glossary

![food1](https://raw.githubusercontent.com/openthings-cc/openthings-food/master/art/food1.svg)


* (food2) http://www.w3.org/TR/2004/REC-owl-guide-20040210/food.rdf (demo)

It is (as it states itself) a example Ontology. It defines wide range of wines and various meals. Could be suitable for restaurants.


![food1](https://raw.githubusercontent.com/openthings-cc/openthings-food/master/art/food1.svg)


* (food3) http://purl.org/foodontology

As it states:

`The Food Ontology is an extension of GoodsRelations Ontology [GoodsRelations] created to represent food and food products. 
Food Ontology describes food products and provides information on ingredients, additives, nutrition facts and other food-specific facts.`

*Note 'GoodsRelations' is actually GoodRelations not some other deviation.*

It has a few classes and basic properties on top of GoodRelations.
It has a set of food additives however much less than (food1). 
What is nice is that it is based on GoodRelations which is by far the most adopted Ontology in the industrial world.
This strategy is also good because GoodRelations is included in most of the e-commerce related solutions now-a-days.

![food1](https://raw.githubusercontent.com/openthings-cc/openthings-food/master/art/food1.svg)


* Agrovoc

is a huge vocabulary describing related to agriculture. 
It is based on skos and thus nicely extensible.
Its size however makes it difficult to adopt. 
As for specific needs one may use just a small part of theat vocabury but miss most of the particular needs there might be.
It is very nice however as a glossary to build up the things one may need in the field of agriculture. 


* DBPedia

pretty nice to link to but not sufficient to use for 
specific need as in this case. DBpedia define topics not product 
services or alike. Also classes hierarchy may be too strict for some 
and too informal or even inaccurate for others as some individual elemts 
may well be defined as classes and vice versa(this comes form the 
origin of DBpedia being based on wikipedia pages and entries in 
general) 


* WikiData 
similar to DBPedia as regards to origin however 
establishing better 'class' hierarchy although in a different way but 
similar to the way Agrovoc is implementing its hirachy. In WikiData 
all 'things' are Items and all items has WikiData 
specific property to define a subclass similarly to skos Concepts and
broader property. WikiData also has not Human friendly names rather 
numbers, which I personally do not like as without using specific 
tools one cannot read/write data smoothly.
 
 

 