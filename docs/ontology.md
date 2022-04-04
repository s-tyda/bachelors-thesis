# Movie
Properties and fields:
- id
- Award (oddzielna klasa)
- Keyword (genre/subject/tag np "Komedia", "Eksploracja kosmosu", "Space Opera")
- Rating (7+/12+/16+ itd.)
- Title
- Ranking (np ocena z IMDB lub Filmwebu)
- originalLanguage
- originalReleaseYear
- associatedLocation (zarówno lokacja fabularna jak i filmowania oraz kraj, jest to oddzielna klasa)
- approximateLength
- cost
- relatedCompany (zarówno dystrybutor jak i producent)
- relatedTo (powiązania z innymi filmami typu prequel/sequel/reboot etc.)
- Contributor (każda osoba powiązana, aktor jak i członek zespołu,
jeśli ktoś ma kilka ról, to ma rekord na każde pole, klasa Person)

# Person
Properties and fields:
- id
- name
- country, birthplace (klasy lokacji)
- gender
- dateOfBirth, dateOfDeath

# Location
Properties and fields:
- id
- name
- countryCode
- coords (współrzędne)
- fictional (bool czy fikcyjna czy prawdziwa)

# Group (uniwersum, franchise etc. - zbiór filmów)
Properties and fields:
- id
- type (typ grupy)
  - uniwersum/franchise/brand (Star Wars/MCU/Lego)
  - postać (np Sherlock Holmes)
  - Ad Hoc (inne)
- members (każdy członek to id jakiegoś filmu)

# Award (może być powiązana zarówno z osobą jak i filmem, np relacjami isNominated albo isWinner)
- year
- type
- name