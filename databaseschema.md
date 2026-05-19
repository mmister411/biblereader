## Table `alephbet`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `Letter_Name` | `text` |  Nullable |
| `Picture` | `text` |  Nullable |
| `Hebrew_Letter` | `text` | Primary |
| `Modern_English` | `text` |  Nullable |
| `Hebrew_Gematria` | `int8` |  Nullable |
| `Meanings` | `text` |  Nullable |
| `Background` | `text` |  Nullable |

## Table `ancient_language_inflected_unaccented_concordance`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary Identity |
| `word` | `text` |  Nullable |
| `lang` | `text` |  Nullable |
| `stopword` | `bool` |  Nullable |
| `VerseRef` | `text` |  Nullable |
| `RowNum` | `float8` |  Nullable |

## Table `ancient_language_words`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary Identity |
| `senses` | `text` |  Nullable |
| `Strongs` | `text` |  Nullable |
| `BDB_Thayers` | `text` |  Nullable |
| `word` | `text` |  Unique |
| `coefficient0` | `float8` |  Nullable |
| `StrongsDef` | `text` |  Nullable |
| `stopword` | `bool` |  Nullable |
| `ConcordEnglish` | `text` |  Nullable |
| `lang` | `text` |  Nullable |
| `RankWord` | `float8` |  Nullable |

## Table `bible_books`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `Author_Audience` | `text` |  Nullable |
| `Author_Name` | `text` |  Nullable |
| `Author_Purpose` | `text` |  Nullable |
| `Authorship_Time` | `text` |  Nullable |
| `Book_Name` | `text` |  Unique |
| `Book_Name_Greek` | `text` |  Nullable |
| `Book_Name_Hebrew` | `text` |  Nullable |
| `Book_Name_Latin` | `text` |  Nullable |
| `Book_Number` | `int8` | Primary |
| `Chapter_Count` | `int8` |  Nullable |
| `Chapter_Outline_Summary` | `text` |  Nullable |
| `Jesus_In_This_Book` | `text` |  Nullable |
| `Key_Doctrines` | `text` |  Nullable |
| `Key_Events` | `text` |  Nullable |
| `Key_Themes` | `text` |  Nullable |
| `Key_Verses` | `text` |  Nullable |
| `Key_Words` | `text` |  Nullable |
| `Literary_Genre` | `text` |  Nullable |
| `Main_Characters_List` | `text` |  Nullable |
| `Mister_Short_Devotional_Introductory_Paragraph` | `text` |  Nullable |
| `Section` | `text` |  Nullable |
| `Subsection` | `text` |  Nullable |
| `Summary_Symbolic_Imagery` | `text` |  Nullable |
| `Top10xRef` | `text` |  Nullable |
| `TypeGroup` | `text` |  Nullable |
| `TypeGroupFeatures` | `text` |  Nullable |
| `TypeGroupThemes` | `text` |  Nullable |

## Table `bible_characters`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary |
| `id1` | `text` |  Nullable |
| `name` | `text` |  Nullable |
| `father` | `text` |  Nullable |
| `name_modern` | `text` |  Nullable |
| `name_hebrew` | `text` |  Nullable |
| `name_greek` | `text` |  Nullable |
| `name_latin` | `text` |  Nullable |
| `name_meaning` | `text` |  Nullable |
| `pronunciation` | `text` |  Nullable |
| `testament` | `text` |  Nullable |
| `major_role_in_bible` | `text` |  Nullable |
| `overview_statement` | `text` |  Nullable |
| `summary` | `text` |  Nullable |
| `lessons_from_their_life` | `text` |  Nullable |
| `interesting_facts` | `text` |  Nullable |
| `archeological_finds` | `text` |  Nullable |
| `occupations` | `text` |  Nullable |
| `titles_held` | `text` |  Nullable |
| `roles_titles` | `text` |  Nullable |
| `notable_traits` | `text` |  Nullable |
| `virtues` | `text` |  Nullable |
| `vices` | `text` |  Nullable |
| `key_verses` | `text` |  Nullable |
| `scripture_mentions` | `text` |  Nullable |
| `character_main_events` | `text` |  Nullable |
| `mother` | `text` |  Nullable |
| `spouses` | `text` |  Nullable |
| `children` | `text` |  Nullable |
| `siblings` | `text` |  Nullable |
| `ancestors` | `text` |  Nullable |
| `descendants` | `text` |  Nullable |
| `links_to_jesus` | `text` |  Nullable |
| `ethnicity_nationality` | `text` |  Nullable |
| `tribe_of_israel` | `text` |  Nullable |
| `genealogy` | `text` |  Nullable |
| `house_line` | `text` |  Nullable |
| `birth_year` | `text` |  Nullable |
| `death_year` | `text` |  Nullable |
| `birth_date` | `text` |  Nullable |
| `death_date` | `text` |  Nullable |
| `death_cause` | `text` |  Nullable |
| `age_estimate` | `text` |  Nullable |
| `reign_or_activity_start` | `text` |  Nullable |
| `reign_or_activity_end` | `text` |  Nullable |
| `location_birth` | `text` |  Nullable |
| `location_death` | `text` |  Nullable |
| `primary_locations` | `text` |  Nullable |
| `primary_scripture_refs` | `text` |  Nullable |
| `secondary_scripture_refs` | `text` |  Nullable |
| `key_events` | `text` |  Nullable |
| `works_or_acts` | `text` |  Nullable |
| `sins_or_failures` | `text` |  Nullable |
| `warnings_or_lessons` | `text` |  Nullable |
| `covenant_context` | `text` |  Nullable |
| `prophecies_related` | `text` |  Nullable |
| `typology_or_foreshadowing` | `text` |  Nullable |
| `theological_themes` | `text` |  Nullable |
| `cultural_context` | `text` |  Nullable |
| `artifacts_or_sites` | `text` |  Nullable |
| `allies` | `text` |  Nullable |
| `opponents` | `text` |  Nullable |
| `mentors` | `text` |  Nullable |
| `mentees` | `text` |  Nullable |
| `legacy_impact` | `text` |  Nullable |
| `application_points` | `text` |  Nullable |
| `timeline` | `text` |  Nullable |
| `cross_refs_ot` | `text` |  Nullable |
| `cross_refs_nt` | `text` |  Nullable |
| `external_sources` | `text` |  Nullable |
| `memory_hook` | `text` |  Nullable |
| `open_questions` | `text` |  Nullable |
| `notes` | `text` |  Nullable |

## Table `bible_locations_geopandas`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary |
| `Name` | `text` |  Nullable |
| `description` | `text` |  Nullable |
| `timestamp` | `text` |  Nullable |
| `begin` | `text` |  Nullable |
| `end` | `text` |  Nullable |
| `altitudeMode` | `text` |  Nullable |
| `tessellate` | `int8` |  Nullable |
| `extrude` | `int8` |  Nullable |
| `visibility` | `int8` |  Nullable |
| `drawOrder` | `text` |  Nullable |
| `icon` | `text` |  Nullable |
| `geometry` | `text` |  Nullable |

## Table `bible_passages`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary Identity |
| `VerseRef` | `text` |  |
| `RowNum` | `int8` |  |
| `Passage` | `text` |  Nullable |
| `abbreviations` | `text` |  |
| `bible_version_FK` | `int8` |  |

## Table `bible_verses`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `JesusMinsitryEvent` | `text` |  Nullable |
| `Book_Number` | `int8` |  Nullable |
| `ContainsLogicProposition` | `bool` |  Nullable |
| `GodIsAttr` | `text` |  Nullable |
| `RowNum` | `int8` | Primary |
| `BookNum` | `int8` |  Nullable |
| `labels` | `text` |  Nullable |
| `Book_Name` | `text` |  Nullable |
| `JesusMinistryOrderID` | `text` |  Nullable |
| `VerseRef` | `text` |  Unique |
| `GodIsOrder` | `text` |  Nullable |
| `coefficient0` | `float8` |  Nullable |
| `Chapter_Count` | `int8` |  Nullable |
| `title` | `text` |  Nullable |
| `TypeGroup` | `text` |  Nullable |
| `Literary_Genre` | `text` |  Nullable |
| `Author_Audience` | `text` |  Nullable |
| `GroupNum2` | `int8` |  Nullable |
| `TSKmain` | `text` |  Nullable |
| `RankVerse` | `float8` |  Nullable |
| `Author_Name` | `text` |  Nullable |
| `Authorship_Time` | `text` |  Nullable |
| `Chapter` | `int8` |  Nullable |
| `Section` | `text` |  Nullable |
| `Subsection` | `text` |  Nullable |

## Table `bible_versions`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary |
| `abbreviation` | `text` |  Nullable |
| `full_name` | `text` |  Nullable |
| `language` | `text` |  Nullable |
| `has_strongs` | `text` |  Nullable |
| `copyright_status` | `text` |  Nullable |

## Table `bible_xrefs`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary Identity |
| `terms` | `text` |  Nullable |
| `weight` | `float8` |  Nullable |
| `connectid` | `text` |  Nullable |
| `source_VerseRef` | `text` |  Nullable |
| `target_VerseRef` | `text` |  Nullable |

## Table `book_abbreviations`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `pk` | `int8` | Primary |
| `Book_Abr` | `text` |  Nullable |
| `Book_Name` | `text` |  |

## Table `hebrew_digraphs`

### Columns

| Name | Type | Constraints |
|------|------|-------------|
| `BiRoot` | `text` | Primary |
| `BiRootStrongs` | `int8` |  Nullable |
| `ConcreteUsage` | `text` |  Nullable |
| `OtherUsage` | `text` |  Nullable |
| `PictoStatement` | `text` |  Nullable |
| `RootMeaning` | `text` |  Nullable |

