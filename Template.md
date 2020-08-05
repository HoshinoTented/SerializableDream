# Template

newtype Identity = String;
newtype FullName = String;

data Quality = Darkness | Aka | Midori | Ao | Shiny

newtype Skills =  [Skill]
newtype SpecialSkill = Skill

## Item

data Item = Item {
    id: Identity,
    name: FullName,
    quality: Quality,
    skills: Skills,
    sskill: SpecialSkill
}

Field    | Value
:--------|:-------------
id       | _|_
name     | _|_
quality  | _|_
skills   | _|_
sskill   | _|_

## Skill

fromDesc :: String -> Maybe SkillAction

data SkillAction = {- Built-in -}
data SkillBody = Auto SkillAction | Skill SkillAction
data Skill = Skill {
    id: Identity,
    name: FullName,
    body: SkillBody
}

Field    | Value
:--------|:------------
id       | _|_
name     | _|_
body     | _|_