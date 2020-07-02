# Atlas Project - Json Files
This are the responses that the Atlas API gives if used the queries bellow:
  
   1- Get Atlas Repository Information: (output: RepositoryInfo)
      https://atlas.linkconsulting.com/rest/repository/list/?filter=[where][name][eq][ `<repositoryName>` ]
      
   2- Get Business Process Information: (output: SearchedBusinessProcessInfo)
      https://atlas.linkconsulting.com/rest/object/list/?filter=[where][objectClass.repository.id][eq][ `<repositoryId>` ],[where][objectClass.name][eq][Business%20Process],[where][name][eq][ `<businessProcessName>` ]
   
   3- Get Process Object Information: (output: depends on the Id given, it can be any of the other files)
      https://atlas.linkconsulting.com/rest/object/properties/list?filter=[where][object.id][eq][ `<IdOfComponentNeeded>` ]

The order from the previous enumeration needs to be followed, since one query gives up the information needed to execute the next one.
