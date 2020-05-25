# Name Breakdown
## Description:

In Mexico it is usual to capture the first name (with middle name when applicable) and the surname (with the father’s surname and the mother’s surname) in a separate way. In the case of transparency obligations, it is mandatory to publish these data in separate fields. Likewise, we need to maintain the name of an organization in another separate field, in order to diference them with individuals.

## Proposal:

### Codelists:

  - legalPersonality
    - naturalPerson
    - legalPerson
    
### Schema:
  - Identifier {object}
    - legalPersonality (string, null) (codelist)
    - givenName (string, null)
    - patronymicName (string, null)
    - matronymicName (string, null)
  - contactPoint {object}
    - contactPointType (string, null) (codelist)
    - givenName (string, null)
    - patronymicName (string, null)
    - matronymicName (string, null)

## Defining texts:


**Code** | **Title** | **Description**
--|--|--
legalPersonality | Legal personality | Specify the legal personality of the entity who participates in this contracting process. Using the [legalPersonality](https://github.com/INAImexico/ocds_nameBreakdown_extension/blob/master/codelists/legalPersonality.csv) codelist.
naturalPerson | Natural person | A natural person is a human entity, as opposed to a legal person, which may be a private or public organization. 
legalPerson | Legal person | A legal person is a non-human entity, which is authorized by law with duties and rights and is recognized as a legal entity.
givenName | Given name | The given name of the natural person.
patronymicName | Patronymic name | The patronymic name of the natural person. This could be used to capture the common surname of a natural person or the first surname for hispanic countries (usually the father's surname).
matronymicName | Matronymic name | The matronymic name of the natural person. This is for the second surname in hispanic countries (usually the mother's surname).

## Issues 

Report issues for this extension in the [standard repository](https://github.com/open-contracting/standard/issues/637) of the Open Contracting Partnership.
