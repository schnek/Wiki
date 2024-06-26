---
title: locales_quest
type: worlddb
category: L
layout: single_markdown
---

# locales_quest
This table contains the localization for the quest texts [quest_properties](/Wiki/database/world/quest_properties/ "Quest properties").

## Structure

Field                                                                                               | Type       | Default | Comment
--------------------------------------------------------------------------------------------------- | ---------- | ------- | -------
[entry](#entry)                                                                                     | int(30)    |         |        
[language_code](#language_code)                                                                     | varchar(5) | 0       |        
[Title](#Title)                                                                                     | text       | 0       |        
[Details](#Details)                                                                                 | text       | 0       |        
[Objectives](#Objectives)                                                                           | text       | 0       |        
[CompletionText](#CompletionText)                                                                   | text       | 0       |        
[IncompletionText](#IncompletionText)                                                               | text       | 0       |        
[EndText](#EndText)                                                                                 | text       | 0       |        
[ObjectiveText1](#ObjectiveText_1_4)                                                                | text       | 0       |        
[ObjectiveText2](#ObjectiveText_1_4)                                                                | text       | 0       |        
[ObjectiveText3](#ObjectiveText_1_4)                                                                | text       | 0       |        
[ObjectiveText4](#ObjectiveText_1_4)                                                                | text       | 0       |        

### entry

The entry ID of the quest from [quest_properties](/Wiki/database/world/quest_properties/ "Quest properties") table.

### language_code

The lanuguage code:

Locale   | Name                         |
-------- | ---------------------------- |
koKR     | Korean                       |
frFR     | French                       |
deDE     | German                       |
zhCN     | Chinese                      |
zhTW     | Taiwanese                    |
esES     | Spanish (EU)                 |
esMX     | Spanish (Latin American)     |
ruRU     | Russian                      |

### Title

The localized Title.

### Details

The localized Details.

### Objectives

The localized Objectives.

### CompletionText

The localized CompletionText.

### IncompletionText

The localized IncompletionText.

### EndText

The localized EndText.

### ObjectiveText_1_4

The localized ObjectiveTexts.