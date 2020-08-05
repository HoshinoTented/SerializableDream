# Template

newtype Identity = String;
newtype FullName = String;

data Quality = BoroBoro | Aka | Midori | Ao | KiraKira

newtype Skills =  [Skill]
newtype SpecialSkill = Skill

## Item

data Item = Item {
    id: Identity,
    name: FullName,
    quality: Quality,
    single: Bool,
    skills: Skills,
    sskill: Maybe SpecialSkill
}

Field    | Value
:--------|:-------------
id       | _|_
name     | _|_
quality  | _|_
single   | _|_
skills   | _|_
sskill   | _|_

## Skill

fromDesc :: String -> Maybe SkillAction

newtype Cost = Cost Integer
data SkillAction = {- Built-in -}
data SkillBody = Auto SkillAction | Skill Cost SkillAction
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