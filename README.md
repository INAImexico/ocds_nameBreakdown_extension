# Name Breakdown
## Description:

In Mexico it is usual to capture the first name (with middle name when applicable) and the surname (with the father’s surname and the mother’s surname) in a separate way. In the case of transparency obligations, it is mandatory to publish these data in separate fields. Likewise, we need to maintain the name of an organization in another separate field, in order to diference them with individuals.

## Proposal:

### Codelists:

  - juridicalPersonhood
    - naturalPerson
    - legalPerson

  - contactPointType
    - contactPoint
    - attorney
    
### Schema:
  - Identifier {object}
    - juridicalPersonhood (string, null) (codelist)
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
juridicalPersonhood | Juridical personhood | Specify the juridical personhood of the entity that participates in this contracting process. Using the [juridicalPersonhood](https://github.com/INAImexico/ocds_nameBreakdown_extension/blob/master/codelists/juridicalPersonhood.csv) codelist.
naturalPerson | Natural person | A natural person is a human entity, as opposed to a legal person, which may be a private or public organization. 
legalPerson | Legal person | A legal person is a non-human entity, which is authorized by law with duties and rights and is recognized as a legal entity.
givenName | Given name | The given name of the natural person.
patronymicName | Patronymic name | The patronymic name of the natural person.
matronymicName | Matronymic name | The matronymic name of the natural person.
contactPointType | Contact point type | Specify the contact point type using the [contactPointType](https://github.com/INAImexico/ocds_nameBreakdown_extension/blob/master/codelists/contactPointType.csv) codelist. 
contactPoint | Contact point | Person who serves as the point of contact for this organization.
attorney | Attorney | The attorney-in-fact is the individual who has an authorization to represent or act on another's behalf in private affairs, business, or some other legal matter.

## Issues 

Report issues for this extension in the [standard repository](https://github.com/open-contracting/standard/issues/637) of the Open Contracting Partnership.
