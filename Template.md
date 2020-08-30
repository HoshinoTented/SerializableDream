# Template

newtype Identity = String
newtype FullName = String
newtype Description = String

data Quality = BoroBoro | Aka | Midori | Ao | KiraKira

newtype Skills =  [Skill]
newtype SpecialSkill = Skill

## Item

data Item = Item {
    id :: Identity,
    name :: FullName,
    desc :: Description,
    quality :: Quality,
    single :: Bool,
    skills :: Skills,
    sskill :: Maybe SpecialSkill
}

Field    | Value
:--------|:-------------
id       | _|_
name     | _|_
desc     | _|_
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
    id :: Identity,
    name :: FullName,
    body :: SkillBody
}

Field    | Value
:--------|:------------
id       | _|_
name     | _|_
body     | _|_

## Chars

newtype Power = Power Integer
newtype MahouPower = MahouPower Integer
newtype MaRyoku = MaRyoku Integer
newtype HealthPower = HealthPower Integer
newtype BrainPower = BrainPower Integer
newtype Shield = Shield Integer
newtype MahouShield = MahouShield Integer
newtype BrainShield = BrainShield Integer
newtype Heal = Heal Integer
newtype Luck = Luck Integer

data Properties = Properties
    Power
    MahouPower
    MaRyoku
    HealthPower
    BrainPower
    Shield
    MahouShield
    BrainShield
    Heal
    Luck

data Chars = Chars {
    id :: Identity,
    name :: FullName,
    properties :: Properties,
    skills :: Skills
}

Field      | Value
:----------|:--------
id         | _|_
name       | _|_
properties | _|_
skills     | _|_