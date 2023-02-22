classDiagram
direction BT
class AchievementChallengeCategory {
   text AchievementCategory
}
class AchievementChallenges {
   text AchievementCategory
   text ProgressExperience
   text ChallengeID
}
class AchievementCriteria {
   string KnowledgeSubject
   text KnowledgeAction
   text KnowledgeCategory
   text PrerequisiteLockID
   integer Occurances
   integer Timespan
   text AwardOnUnlock
   text EvaluationRule
   text AcknowledgeOnID
   text AcknowledgeOffID
   integer PrereqSubjectsKnown
   text TransferOneOfEach
   text AchievementID
}
class AchievementDefinition {
   text AchievementType
   text AlternateID
   text OneOfEachInit
   integer SaveOnUpdate
   text AchievementID
}
class AchievementDynamic {
   text AchievementID
   int Instances
   int IsComplete
   text OneOfEach
   integer RewardsDelayed
}
class AchievementRewardCategory {
   text RewardCategory
}
class AchievementRewardTypes {
   text RewardType
}
class AchievementRewards {
   text AchievementID
   text RewardType
   text RewardText
   integer RewardInt
   boolean IsHidden
   integer Priority
   integer Delayed
   text RewardCategory
}
class AchievementTypes {
   text AchievementType
}
class AcknowledgementDynamic {
   integer MaxCount
   integer CurrentCount
   text AcknowledgementID
   text Value
}
class AcknowledgementMissionDisablesVO {
   text MissionID
}
class AcknowledgementMissionStats {
   text MissionStatus
   text MissionID
}
class AcknowledgementNPCType {
   text NPCType
}
class AcknowledgementRules {
   text TemporaryEventID
   text RuleType
   integer Score
   text NPCType
   text TogglingSystem
   integer MaxCount
   integer Cooldown
   boolean PlayInExclusiveMission
   text VOEventID
}
class ActivityCriticalResult {
   integer HousePoints
   integer BaseChance
   integer ProfessorChanceAdjust
   text ProfessorHouse
   integer PerkChanceAdjust
   text PerkAction
   text PerkFocus
   text PerkBuff1
   text PerkBuff2
   text PerkBuff3
   text SubjectID
   text ResultType
}
class ActivityDefinition {
   text ActivityTypeID
   integer StartTime
   integer EndTime
   text SubjectID
   text LocationID
   text SeasonID
   text ActivityRecurrenceTypeID
   integer WeekNumber
   boolean Sunday
   boolean Monday
   boolean Tuesday
   boolean Wednesday
   boolean Thursday
   boolean Friday
   boolean Saturday
   text ActivityID
}
class ActivityRecurrenceTypes {
   text ActivityRecurrenceTypeID
}
class ActivityTypes {
   real TravelTimeFactor
   text OutfitTypeID
   text ActivityTypeID
}
class ActorDefinition {
   text GenderID
   text AdditionalVoiceID
   text EmoteVoiceID
   text SkeletonTypeID
   text RegistryID
}
class AmbientChatterTopicsDynamic {
   integer Active
   integer MissionLocked
   string TopicID
}
class AmbientCreatureDefinition {
   double MinSpawnRange
   double MaxSpawnRange
   double CullRange
   integer MinClusterSize
   integer MaxClusterSize
   double ClusterRadius
   text CreatureID
}
class AmbientCreatureFrequencyDefinition {
   real NumPerHectare
   text Frequency
}
class AmbientCreatureGroup {
   text GroupID
}
class AmbientCreatureGroupDefinition {
   text GroupID
   text CreatureID
   text Frequency
   double ClusterProbability
}
class AncientMagicLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class AvatarFullBodyPresetsDynamic {
   text PresetName
   text RegistryId
   text PresetType
}
class BanditCampLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class BeaconDataDynamic {
   text BeaconName
   text BeaconType
   integer ParentUID
   integer BeaconState
   real WorldX
   real WorldY
   real WorldZ
   text LocationID
   integer BeaconUID
}
class BeaconDefinition {
   text Name
}
class BeastDenLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class BiomeType {
   text BiomeTypeID
}
class BrewingSiteDynamic {
   integer StationUID
   integer BrewingState
   text PotionID
   integer UncollectedYield
   integer LastUpdateTime
   double ProgressAtLastUpdate
   integer SiteUID
}
class BrewingUICategories {
   text Category
}
class BroomActionSplineDynamic {
   int TaskIndex
   real XPos
   real YPos
   real ZPos
   string GUID
}
class BroomRaceDefinition {
   string RaceName
}
class BroomRaceTimesDynamic {
   real BestTime
   boolean MissionRelevant
   string RacerName
   unknown RaceName
}
class BuffActionType {
   text ActionID
}
class BuffAttributeType {
   text ActionID
   text FocusID
   text AttributeID
}
class BuffDefinition {
   text BuffID
}
class BuffFocusType {
   text FocusID
}
class BuffSlotsDynamic {
   text CharacterID
   text AttributeID
   integer SlotNo
   real Amount
   real Percentage
   real Ticks
   text SourceID
   real Interval
   text IntervalEffect
   real LastInterval
   integer EntryID
}
class BuffsDynamic {
   text CharacterID
   text AttributeID
   real Units
   real Percentage
   text ActionID
   text FocusID
   integer EntryID
}
class CharacterDefinition {
   text HouseID
   text IdentityID
   text FactionID
   integer Year
   text SocialHeritage
   text SocioEconomicStatus
   integer RealizationFidelity
   text CopyScheduleFromCharacterID
   text RestrictToLocation
   text BirthdaySeason
   integer BirthdayDate
   text LootDrop
   integer AlwaysProtected
   text CompanionLock
   text CharacterID
}
class CharacterEmoteVoices {
   text EmoteVoiceID
}
class CharacterItemTypes {
   real OrderID
   boolean CanBeEmpty
   text SocketName
   text CharacterItemTypeID
}
class CharacterLoadoutsDynamic {
   text DefaultSpell
   text CombatSpell1
   text CombatSpell2
   text CombatSpell3
   text CombatSpell4
   text CombatSpell5
   text CombatSpell6
   text Name
}
class CharacterLookOverrideDynamic {
   text OverrideRegistryID
   text RegistryID
}
class CharacterOutfitTypes {
   text OutfitTypeID
   text SubtypeID
}
class CharacterVoices {
   text VoiceID
}
class CharactersDynamic {
   text CharacterID
   integer CompanionBondingPoints
   integer DailyGiftCount
   integer DailyKnowledgeAskCount
   real AskedForFavor
   text FavorIdentity
   real BeingExtorted
   text ExtortionIdentity
   integer PlayerGainedSoCap
   text Identity2
   text Identity3
   real UnderImperiusCurse
}
class CollectionActions {
   text LockID
   text SubjectID
   text KnowledgeAction
   text ItemID
   text CollectionState
}
class CollectionCategories {
   text CategoryID
}
class CollectionDynamic {
   text CategoryID
   text SubcategoryID
   text ItemID
   text ItemState
   integer UpdateTime
}
class CollectionItems {
   text CategoryID
   text SubcategoryID
   text ProductID
   text StateAtNewGame
   text AOCLock
   text HouseExclusive
   text ItemID
}
class CollectionStates {
   text CollectionState
}
class CollectionSubcategories {
   text SubcategoryID
}
class CombatVolumeGroupDynamic {
   text DOVGUID
   text CombatVolumeGroupID
}
class CompanionBondingLevels {
   integer BondingLevelMaxPoints
   integer BondingLevel
}
class CompanionStatsConditionDefinition {
   text ConditionID
}
class CompanionStatsTriggerTypes {
   text Type
}
class CompanionStatsTriggersDynamic {
   text StatID
   text Condition
   integer ReferenceValue
   text VoiceOverEvent
   integer TriggerCount
   text TriggeredCompanions
   text TriggerType
   text RuleName
}
class ConjurationCategory {
   text ParentCategory
   integer SortingIndex
   text ConjurationCategory
}
class ConjurationContext {
   integer ConjurationBudget
   real MainAreaBudgetRatio
   text ConjurationContext
}
class ConjurationContextDefinition {
   text ConjurationContext
   text ConjurationCategory
}
class ContainerMaxSlots {
   integer MaxSlots
   text ContainerID
}
class ConversationDynamic {
   integer TimesPlayed
   text CharacterID
   text ConversationName
}
class ConversationExclusiveDynamic {
   text CharacterID
   text EventNamePattern
   text RegisteredByMission
}
class ConversationThreadDynamic {
   integer IntegerValue
   string StringValue
   string PropertyName
}
class CreatureAttributeFacts {
   text CreatureID
   text CreatureAttributes
}
class CreatureColorVariation {
   text ColorVariation
}
class CreatureColorVariationBreeding {
   text ParentVariation1
   text ParentVariation2
   text ChildVariation
   real ChanceWeight
}
class CreatureColorVariationDefinition {
   text AdultID
   text ColorVariation
   real SpawnChanceWeight
   double MaleScaleVariationMin
   double MaleScaleVariationMax
   double FemaleScaleVariationMin
   double FemaleScaleVariationMax
}
class CreatureDefinition {
   text ByProduct
   integer ByproductHarvestCount
   double ByproductProductionTimeSec
   text PreferredToy
   double PlayWithToyHappinessPercentage
   text Conflict1
   text Conflict2
   boolean CanBeCaptured
   text AchievementForCapturing
   integer CompletedYearForCapture
   double CapturingTime
   integer CapturingGates
   integer CapturingDistanceMax
   boolean OnlyCapturableWhenNearDeathKneeling
   boolean isCarnivore
   boolean isAgressive
   integer BaseEconomyValue
   double SpawnFlyingProbability
   double MinShutdownDistance
   double MaxShutdownDistance
   double RenderShutdownDistance
   text CreatureID
}
class CreatureDefinitionMap {
   text EnemyClass
   text RegistryID
}
class CreatureFamilies {
   text OffspringID
   text EggID
   integer PregnancyDurationSecs
   integer ChildhoodDurationSecs
   integer HatchingDurationSecs
   text AdultID
}
class CreaturePersistenceDynamic {
   integer ParentUID
   integer ObjectID
   integer EInteractiveState
   real Health
   real XPos
   real YPos
   real ZPos
   real ZRot
}
class CreatureUIDMappingDynamic {
   integer CreatureUID
   integer ParentUID
   integer ActorIndex
}
class CrimeEnforcementMatrix {
   double CallAF
   double Flee
   double Retaliate
   string EnforcementKey
}
class CrimeMiscData {
   string Value
   string Key
}
class CrimeSceneDurations {
   string CrimeType
   string Severity
   integer Duration
}
class CrimeSceneInvestigationDurations {
   real Duration
   string Severity
}
class CrimeSceneInvestigationRadius {
   real InvestigationRadiusInMeters
   string Severity
}
class CrimeSceneMaxInvestigators {
   string CrimeType
   string Severity
   integer MaxInvestigators
}
class CrimeSeverityMatrix {
   double TrivialMin
   double TrivialMax
   double LowMin
   double LowMax
   double MediumMin
   double MediumMax
   double HighMin
   double HighMax
   string Crime
}
class CurriculumDynamic {
   text CurriculumID
   integer Year
   text Season
}
class CurriculumEOYRewards {
   integer Year
   text KnowledgeCard
   text Reward
   text UniqueID
}
class CurriculumProfessorDynamic {
   text ProfessorID
}
class CurriculumRewards {
   text Season
   text CurriculumID
   integer Year
   text KnowledgeCard
   text Reward
}
class CurriculumTurnInDefinitions {
   string TurnInType
   text TurnInNPC
   integer Quantity
   text Detail
   text RelatedItem1
   text RelatedItem2
   text RelatedItem3
   text RelatedItem4
   string CurriculumID
   integer Year
   string TurnInID
   integer Tier
}
class CurriculumTurnInDynamic {
   string CurriculumID
   integer Year
   string TurnInType
   string TurnInID
   integer Quantity
   integer Tier
   text RelatedItem1
   text RelatedItem2
   text RelatedItem3
   text RelatedItem4
}
class CurriculumTurnInTypes {
   integer TypeValue
   string TypeID
}
class CurriculumTypes {
   text CurriculumTypeID
}
class CurriculumYear {
   integer Year
}
class DoorStates {
   text State
}
class DoorsDynamic {
   real OpenDirection
   boolean KeepOpen
   text ID
}
class DuelTechniqueCategory {
   text CategoryID
}
class DuelTechniqueDifficulty {
   text DuelTechniqueDifficultyID
}
class DuelTechniqueFirstState {
   text DuelTechniqueFirstStateID
}
class DuelTechniqueRequirementFunction {
   text FunctionID
}
class DuelTechniqueRules {
   text RuleDefinition
   integer Weight
   text RuleID
}
class DuelTechniqueSelectionMaxEncounterWeight {
   integer MaxEncounterWeight
   integer SelectionCount
}
class DuelTechniqueStatsDynamic {
   boolean IsCompleted
   int NumTimesSeen
   text DuelTechniqueID
}
class DuelTechniqueSubtype {
   text DuelTechniqueSubtypeID
}
class DuelTechniques {
   text DTCategory
   double Weight
   text Difficulty
   text DescriptionKey
   text DebugDescription
   text Subtype
   integer CountGoal
   boolean RequiresCombatVolume
   text SpellID_1
   text SpellID_2
   text SpellID_3
   text SpellID_4
   text SpellRequirementFunction
   text EnvironmentObstacleID_1
   text EnvironmentObstacleID_2
   text EnvironmentObstacleID_3
   text ItemID_1
   text ItemID_2
   text ItemID_3
   boolean IsStealthApproachRequired
   text PerkID_1
   text PerkID_2
   text PerkID_3
   text PerkID_4
   text PerkRequirementFunction
   boolean IsHiddenEnemyRequired
   boolean CompletionIgnoresEnemyRequirements
   text DuelTechniqueID
}
class DuelTechniquesEncounterDynamic {
   text CombatVolumeGroupID
   text DuelTechniqueID
   boolean Awarded
   integer ProgressCount
   integer ProgressGoal
   boolean ReRoll
   boolean ProgressFail
   integer TargetTimeLimit
   integer TimeElapsed
}
class DuelTechniquesEnemyEncounterWeightOverrides {
   integer EncounterWeight
   text EnemyID
}
class DuelTechniquesEnemyIDRequirement {
   text DuelTechniqueID
   text EnemyID
   integer MinCount
}
class DuelTechniquesEnemyProperties {
   text Property
}
class DuelTechniquesEnemyPropertyRequirement {
   text DuelTechniqueID
   text Property1
   text Property2
   integer MinCount
}
class DuelTechniquesLocks {
   text DuelTechniqueID
   text LockID
   boolean CheckUnlocked
}
class DuelTechniques_ComboColumns {
   text InitialState
   text FinishingSpellID_1
   text FinishingSpellID_2
   text FinishingSpellID_3
   text DuelTechniqueID
}
class DuelTechniques_CountGoalOverrides {
   text DuelTechniqueID
   integer MinEnemyCount
   integer CountGoal
}
class DuelTechniques_CustomEventColumns {
   text EventGameplayTag
   text DuelTechniqueID
}
class DuelTechniques_DamageColumns {
   boolean HasKillReq
   boolean HasAMReq
   boolean HasTransformReq
   text ImpactGameplayTags
   text DamageSpellID_1
   text DamageSpellID_2
   text DamageSpellID_3
   text DamageSpellID_4
   text ProxyInstigatorClass
   text ObjectVictimClass
   text DuelTechniqueID
}
class DuelTechniques_DepulsoColumns {
   text LaunchActor
   text TargetActor
   text LaunchActorState
   text DuelTechniqueID
}
class DuelTechniques_OppugnoColumns {
   string ValidObjectNames
   boolean EnforceTargetRequirement
   text DuelTechniqueID
}
class DuelTechniques_ReactionColumns {
   string StartAbilities
   string DuelTechniqueID
}
class DuelTechniques_SpellEffectColumns {
   text ImpactGameplayTags
   text AffectingSpellID_1
   text AffectingSpellID_2
   text AffectingSpellID_3
   text DuelTechniqueID
}
class DuelTechniques_TimedEncounterOverrides {
   integer NumSeconds
   text EnemyID
}
class DuelTechniques_TimedJuggleColumns {
   integer GoalTime
   integer EnemyCount
   text DuelTechniqueID
}
class DungeonChestLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   string Owner
   string Name
}
class DungeonDataDynamic {
   text DataBlob
   text DungeonID
}
class DungeonEntrances {
   integer EntranceIndex
   real XPos
   real YPos
   real ZPos
   real ZRot
   real BeaconXPos
   real BeaconYPos
   real BeaconZPos
   integer Ring
   text ReqSpell1
   text ReqSpell2
   text ReqSpell3
   text ReqSpell4
   text ReqSpell5
   text CompletionSpell1
   text CompletionSpell2
   text CompletionSpell3
   text CompletionSpell4
   text CompletionSpell5
   text Resource1
   text Resource2
   text Resource3
   text Resource4
   text Resource5
   text Resource6
   text Resource7
   text Enemy1
   text Enemy2
   text Enemy3
   text Enemy4
   text Enemy5
   text Chest1
   text Chest2
   text Chest3
   text Lore1
   text Lore2
   text Lore3
   text DungeonName
}
class EavesdropCharacters {
   integer NumParticipants
   text Abbreviation
   text RegistryID
}
class EavesdropConversations {
   text Participant1
   text Participant2
   text Participant3
   text Participant4
   text Location
   text ConversationID
}
class EavesdropLocations {
   text Abbreviation
   text LocationID
}
class EconomicExpiryDynamic {
   integer Expiry
   text UniqueID
}
class EncounterExclusions {
   text EncounterGUID
   text EnemyType
   text SubType
}
class EncounterInclusions {
   text EncounterGUID
   text EnemyType
   text SubType
}
class EncounterInstance {
   text Name
   text eModifier
   integer eEnemyLevelCap
   real eEncounterScoreMin
   real eEncounterScoreCap
   integer eEnemyCountCap
   text eStatusCap
   integer SpawnZoneCount
   text World
   text GroupTag
   real XPos
   real YPos
   real ZPos
   text GUID
}
class EncounterScoreModifier {
   integer PlayerEasy
   integer PlayerMedium
   integer PlayerHard
   integer MinLevel
   integer MaxLevel
   text EncounterLevel
}
class EncounterSpawnZones {
   text Encounter
   text Name
   text World
   text GroupTag
   integer eEncounterPercent
   boolean eAllowRanged
   boolean eAllowMelee
   text eSizeCap
   text eSpawnType
   integer eMinCount
   integer eMaxCount
   real eMinCardCost
   real eMaxCardCost
   integer eWeaponPercent
   text eRestriction
   boolean Static
   text DOVGUID
}
class EnemyAccuracyParams {
   real Amount
   real Range
   text Level
}
class EnemyAggressivenessParams {
   real SortDistanceSkew
   real TicketWeight
   real TicketSinceLastAttackWeight
   real TicketOnCameraWeight
   real TicketRandomWeight
   real TicketTargettedWeight
   real NumTicketsScale
   real MinMoveTimePriorToAttack
   real AttackExecuteCooldownChance
   text AttackExecuteCooldownChangeScale
   real AttackExecuteCooldownMin
   real AttackExecuteCooldownMax
   real AttackExecuteCooldownMinAttacks
   real AttackExecuteCooldownMaxAttacks
   text Level
}
class EnemyAgilityParams {
   real MoveChance
   real MoveChanceIncreaseRate
   real NewLocChance
   real NewLocChanceAddDamage
   real NewLocDamageAddTimeout
   real NewLocSuccessCooldown
   real NewLocFailCooldown
   real NewLocMinAngle
   real NewLocMaxAngle
   text Level
}
class EnemyAttackData {
   real BaseWeight
   real RandomWeight
   boolean ExcludeAttackWeight
   boolean IgnoreHistory
   real Damage
   text DamageLevel
   boolean UnblockableByPlayer
   text UnblockableByNPC
   real PositionPriority
   real AttackDistMin
   real ApproachDistMin
   real ApproachDistMax
   real ApproachDistDefer
   real AttackDistMax
   real ApproachTolerance
   real AttackTolerance
   integer ImmediateOnly
   real SelectProbability_1
   real SelectMin_1
   real SelectMax_1
   real SelectProbability_2
   real SelectMin_2
   real SelectMax_2
   real SelectProbability_3
   real SelectMin_3
   real SelectMax_3
   real SelectFallbackCloser
   real SelectFallbackFurther
   real ParryLeadIn
   real ParryToRelease
   real PerryPerfectBegin
   text ParryCounterType
   text ParryResponseType
   text ParryCounterStepDirection
   text ParryCounterStyle
   text ParryDodgeStyle
   real ParryAbortDistance
   real Recovery
   text AttackTicket
   text AttackTicket2
   text AttackTicket3
   text AttackScore
   text ScoreLevel
   unknown 
   real DotDamPerc
   real DotDamDur
   text EnemyID
   text AttackID
}
class EnemyAttackExecuteCooldownScale {
   real Attackers_1
   real Attackers_2
   real Attackers_3
   real Attackers_4
   real Attackers_5
   real Attackers_6
   real Attackers_7
   real Attackers_8
   real Attackers_9
   real Attackers_10
   text Level
}
class EnemyAttackIDs {
   text AttackID
}
class EnemyAttackModifier {
   text AttackerSubTypeID
   text TargetSubTypeID
   real MinOptRange
   real MaxOptRange
   real RangedPercent
   boolean MeleeAllowed
   boolean RangedAllowed
   boolean BallisticAllowed
}
class EnemyAttackParams {
   text ConditionGameplayTag
   real DesynchronizationTime
   real SuccessBreakAdd
   real FailBreakAdd
   real TicketCooldownMin
   real TicketCooldownMax
   real TicketCooldownDeviation
   real GroupCooldown
   real TypeCooldown
   text TicketCooldownScale
   text TicketLevelDiffScale
   real TicketsPerAttacker1
   real TicketsPerAttacker2
   real TicketsPerAttacker3
   real TicketsPerAttacker4
   real TicketsPerAttacker5
   real TicketsPerAttacker6
   real TicketsPerAttacker7
   real TicketsPerAttacker8
   real TicketsPerAttacker9
   real TicketsPerAttacker10
   text AttackTicket
}
class EnemyAttackScore {
   real TypePriorityWeight
   real OffscreenWeight
   real HasAttackedWeight
   real HighlightedWeight
   real CorridorClearWeight
   real RandomWeight
   text Name
}
class EnemyAttackScoreLevel {
   text Name
}
class EnemyAttackSelectionData {
   real LongDistBump
   real ShortDistBump
   real ShieldBreaker
   real CrowdControlEffect
   real DamagePotential
   real CurseApplier
   real JuggleStarter
   real JuggleContinuer
   real JuggleEnder
   real LargeCharInterrupter
   real AOE
   real Fire
   real StupefyAdvancer
   real StupefyEnder
   real PlantPriorityBump
   text AttackName
}
class EnemyAttackSelectionWeights {
   real LongDistBump
   real ShortDistBump
   real ShieldBreaker
   real CrowdControlEffect
   real DamagePotential
   real CurseApplier
   real JuggleStarter
   real JuggleContinuer
   real JuggleEnder
   real LargeCharInterrupter
   real AOE
   real Fire
   real StupefyAdvancer
   real StupefyEnder
   real PlantPriorityBump
   text State
}
class EnemyAttackTicket {
   text AttackTicket
}
class EnemyAttackTicketLevel {
   integer Value
   text Level
}
class EnemyAttackWeights {
   real AttackWeight
   text EnemyID
   text AttackID
   integer EnemyLevel
}
class EnemyCombatPositioningParams {
   real MoveChanceLowerInterval
   real MoveChanceLower
   real MoveChanceUpperInterval
   real MoveChanceUpper
   real MoveChanceStartAngleMin
   real MoveChanceStartAngleMax
   integer TooCloseTargetEnable
   real TooCloseTargetLowerDist
   real TooCloseTargetUpperDist
   integer TooCloseTeammateEnable
   real TooCloseTeammateLowerDist
   real TooCloseTeammateUpperDist
   real RecalculateToTargetDeltaAngle
   real RecalculateTargetDeltaDist
   real AttackAnglePosMax
   real AttackAngleNegMax
   real CloserSearchAddDist
   real CloserAnglePosMax
   real CloserAngleNegMax
   real CloserTooCloseDist
   real CloserAngleWidthMult
   real SegmentExtendDist
   real SegmentTooCloseDist
   real LOSMinCheckDist
   real LOSCheckTime
   real LOSCheckTimeVariance
   text Level
}
class EnemyCombatThreatLevels {
   integer ThreatScoreMin
   integer ThreatScoreMax
   integer ThreatValue
   text CombatThreatLevel
}
class EnemyConfigurationOverrides {
   text EnemyDefinitionID
   text LoadoutID
   text AttackDataID
   text DefenseDataID
   text ScalingDataID
   text CharacterID
   text ContextID
}
class EnemyDamageLevels {
   real DamageValue
   text DamageLevel
}
class EnemyDamageParams {
   real DamageAdjustment
   text Level
}
class EnemyDefenseParams {
   int ShieldAvailableAtLevel
   text DefenseLevel
   integer GetupCounterVsShieldChance
   real GetUpTimeSinceLastAttack
   integer RecoverHitLimit
   real RecoverTimeInReaction
   integer ProtegoConsecutiveDeflectLimit
   integer ApparateAttackCount
   integer CounterAttackDeflectLimit
   integer EscapeHitLimit
   real EscapeHitTime
   integer DodgeRollChance
   text EnemyID
}
class EnemyDefinition {
   boolean IsSpawnable
   boolean IsSE
   real Mass
   real CardScore
   integer Level
   text Size
   boolean Melee
   boolean Ranged
   real OverkillPercent
   real CritHealthPercent
   integer MinSelectRange
   integer MaxSelectRange
   integer RangeFalloff
   text Status
   text CombatPositioning
   text Agility
   text Idle
   text Aggressiveness
   text TicketCooldown
   text Accuracy
   integer Damage
   real Threat
   real Courage
   int AudioPriority
   real MinOptAvDist
   real MaxOptAvDist
   text Drop1
   text Drop2
   text Drop3
   text KilledKnowledgeAction
   text Attribute1
   text Attribute2
   text Attribute3
   text Attribute4
   text Attribute5
   text EnemyID
}
class EnemyDefinitionDuelTechniqueCachedProperties {
   boolean Freezable
   boolean Burnable
   boolean Transformable
   text EnemyID
}
class EnemyDefinitionFallback {
   text ProgressLockID
   text FallbackID
   text RegistryID
}
class EnemyDefinitionGroup {
   text GroupName
   text ClassID
}
class EnemyDefinitionMap {
   text EnemyClass
   text RegistryID
}
class EnemyDefinitionNamed {
   string LootDrop
   text KilledLockID
   text RegistryID
   text ObjectClass
}
class EnemyDefinitionRedirect {
   text RegistryID
   text ObjectClass
}
class EnemyDenLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   string Name
}
class EnemyDifficultyScaling {
   integer Difficulty
   real TicketScale
   real DamageScale
   real HealthScale
   real ParryScale
   real PerfectParryScale
   real ProtegoDeflectCount
   real ProtegoDecayRate
   real ProtegoDamageAdjustment
   real ProtegoCooldownTime
   text Level
}
class EnemyIdle {
   real Idle
   real IdleBreak
   real Taunt
   real Shuffle
   real IdleFallback
   real IdleBreakFallback
   real TauntFallback
   real ShuffleFallback
   text Type
}
class EnemyIdleParams {
   real IdleChance
   real TauntChance
   real ShuffleChance
   real ApparateChance
   text Level
}
class EnemyInteractionTypes {
   text Interaction
}
class EnemyLevelParams {
   integer Value
   text Level
}
class EnemyLevelTicketCooldownScale {
   real Level_0
   real Level_10
   real Level_20
   real Level_30
   real Level_40
   real Level_50
   real Level_60
   real Level_70
   real Level_80
   real Level_90
   real Level_100
   text Type
}
class EnemyParryCounter {
   unknown Type
}
class EnemyParryCounterStyle {
   unknown Style
}
class EnemyParryData {
   real Leadin
   real ReleaseTo
   text EnemyID
   text AttackID
}
class EnemyParryDodge {
   text Style
}
class EnemyParryResponse {
   text Type
}
class EnemyParryStep {
   text Direction
}
class EnemyPerceptionScoreType {
   text Type
}
class EnemyPerceptionScores {
   real DistanceMinWeight
   real DistanceMaxWeight
   real DistanceMin
   real DistanceMax
   real MaintainTargetWeight
   real MaintainTargetFalloff
   real TargetWeight
   real LargeCharacterWeight
   real LevelMultWeight
   real LevelMin
   real LevelMax
   real NumAttackingMultWeight
   real LastDamagedByWeight
   real LastDamagedByFalloff
   real NearDeathKneelingWeight
   real AttackingPlayerWeight
   real AttackingPlayerFalloffSecs
   real ShieldedWeight
   real RemainingHealthWeight
   real Reacting
   real ReactingGround
   real ReactingAir
   real ReactingKnockedDown
   real ReactingRagdoll
   real ReactingCC
   real InReactionShort
   real InReactionMed
   real InReactionLong
   real InReactionMax
   real InCCReaction
   real InKnockDown
   real InRagDoll
   real Cursed
   real Crucioed
   real InAir
   real ShieldsOn
   real Attacking
   real PlayerHighlighted
   real TargettedPlayer
   real ThreatLow
   real ThreatMed
   real ThreatHigh
   real ThreatMax
   real HealthLow
   real HealthMed
   real HealthHigh
   real HealthCritical
   real SpiderOnFire
   real InferiusOnFire
   real InferiusKamikaze
   text Type
}
class EnemyPersistenceDynamic {
   integer EInteractiveState
   real Health
   real XPos
   real YPos
   real ZPos
   real ZRot
   real CharacterLevel
   integer AllowDeadSpawn
   integer ParentUID
   integer ObjectID
}
class EnemyShieldBreaker {
   text Level
}
class EnemyShieldTypes {
   text Type
}
class EnemySize {
   integer Value
   text Type
}
class EnemyStatus {
   integer Value
   text StatusType
}
class EnemySubtypeData {
   integer NumTicketsEasy
   integer AttackedTicketsAddEasy
   integer NumTicketsMedium
   integer AttackedTicketsAddMedium
   integer NumTicketsHard
   integer AttackedTicketsAddHard
   unknown SubtypeID
}
class EnemyTargetSelection {
   real DistNearWeight
   real DistFarWeight
   real DistNear
   real DistFar
   real MaintainTargetWeight
   real MaintainTargetFalloff
   real TargetWeight
   real LargeCharacterWeight
   real NumAttackingMultWeight
   real StayInWeight
   real RecentlyAttackedByWeight
   real RecentlyAttackedByFalloff
   real RecentlyAttackedByPlayerWeight
   real RecentlyAttackedByPlayerFalloff
   real HighlightedByPlayerWeight
   real RecentlyAttackedWeight
   real RecentlyAttackedFalloff
   real RecentlyAttackedPlayerWeight
   real RecentlyAttackedPlayerFalloff
   real ReactingIncMultWeight
   real AttackingWeight
   real ReactingPeakTime
   real ReactingDecMultWeight
   real InCCReactionWeight
   real InKnockDownWeight
   real InRagDollWeight
   real InAirWeight
   real InCriticalHealthWeight
   real InNearDeathKneelingWeight
   real ShieldsOnWeight
   real LevelMultWeight
   real LevelMinWeight
   real LevelMaxWeight
   real HealthMultWeight
   real HealthMinWeight
   real HealthMaxWeight
   real ThreatMultWeight
   real ThreatMinWeight
   real ThreatMaxWeight
   real SpiderOnFireWeight
   real InferiusOnFireWeight
   real InferiusKamikazeWeight
   text Type
}
class EnemyTicketCooldownScale {
   real Attackers_1
   real Attackers_2
   real Attackers_3
   real Attackers_4
   real Attackers_5
   real Attackers_6
   real Attackers_7
   real Attackers_8
   real Attackers_9
   real Attackers_10
   text Type
}
class EnemyTicketLevelDiffScale {
   real TicketLevelsPerInc
   real TicketIncVal
   real TicketMaxInc
   real CooldownDiffInc
   real CooldownDiffMin
   real CooldownDiffMax
   real LeadinDiffInc
   real LeadinDiffMin
   real LeadinDiffMax
   text Type
}
class EnemyVulnerableDamageMods {
   real DefaultDamageScale
   real VulnerableDamageScale
   text EnemyID
   string Difficulty
}
class EnvironmentObstacleTypes {
   text EnvironmentObstacleTypeID
}
class EquippedGearDynamic {
   text GearID
   text GearVariation
   text ActorID
   text SlotID
}
class EvilEffectivenessItems {
   real EffectivenessAdjustment
   text ItemID
}
class ExpansionTentNPCs {
   text StatID
   text CharacterID
}
class ExpansionTents {
   text LocationID
   real EntranceXPos
   real EntranceYPos
   real EntranceZPos
   real ExitXPos
   real ExitYPos
   real ExitZPos
   text TentID
}
class ExperienceActions {
   integer ExperiencePoints
   text ExperienceAction
}
class ExperienceLevels {
   integer PointsForNextLevel
   integer ExperienceLevel
}
class FastTravelLocations {
   boolean Available
   real LocationX
   real LocationY
   real LocationZ
   text WorldName
   boolean IsSaveLocation
   boolean IsFloo
   real ZRot
   boolean IsBuiltNightly
   boolean ShowOnMap
   real BeaconLocationX
   real BeaconLocationY
   real BeaconLocationZ
   text Name
}
class FastTravelRegions {
   unknown RegionID
}
class FastTravelSaveLocations {
   boolean IsSaveLocation
   string Name
}
class FertilizerDefinition {
   integer ExtraYieldAmount
   text FertilizerID
}
class FilterPopulation {
   string CharacterID
}
class ForcedGearAppearanceDynamic {
   text GearAppearanceID
   text GearSlotType
}
class ForegeableCategoryDefinition {
   text Category
}
class GameEventIntensity {
   text EGameEvent_Intensity
}
class GameFeaturesDynamic {
   text key Feature
   text Source
}
class GearAbilityDefinition {
   text IdentityType
   text Level1
   text Level2
   text Level3
   text Level4
   text Level5
}
class GearAbilityWeights {
   real Level1
   real Level2
   real Level3
   real Level4
   real Level5
   integer Tier
}
class GearAppearanceItems {
   text GearAppearanceID
}
class GearGeneration {
   real GearTraitChance
   real IdentifiedChance
   real LevelMin
   real LevelMax
   real OnLevelChance
   text Rarity
}
class GearItems {
   text SlotID
   text GearAppearanceID
   integer NumGeneralAbilities
   text GearID
}
class GearItemsDynamic {
   integer GearLevel
   integer OffenseStat
   integer DefenseStat
   integer CooldownStat
   text GeneralAbility1
   text GeneralAbility2
   text GeneralAbility3
   text GearAppearanceOverrideID
   integer IsIdentified
   integer StatUpgrades
   text GearTags
   text GearID
   text GearVariation
}
class GearPowerLevels {
   integer MinPowerLevel
   integer MaxPowerLevel
   integer EpicStatBonus
   integer LegendaryStatBonus
   integer ExpectedGearLevel
   integer PlayerLevel
}
class GearPowerStats {
   real DamageMultiplier
   real DamageReductionPercentage
   real CooldownReductionPercentage
   integer PowerLevel
}
class GearSlotTypeMapping {
   text SlotID
   text OutfitItemType
}
class GearSlotTypes {
   text DefaultGearID
   text SlotID
}
class GearStatIncrease {
   integer Amount
   text Rarity
   integer Upgrade
}
class GearStatUpgrade {
   integer Cost
   text Rarity
   integer StatType
   int Upgrade
   integer ItemID
}
class GearTraitRecipeDefinition {
   text LockID
   integer SortingIndex
   text Component1
   integer Quantity1
   text Component2
   integer Quantity2
   text Component3
   integer Quantity3
   text Component4
   integer Quantity4
   text Component5
   integer Quantity5
   text Component6
   integer Quantity6
   text RecipeItem
   text GearAbility
}
class Genders {
   text GenderID
}
class GoldChestInfo {
   text ChallengeLocale
   text WorldName
   text LevelName
}
class GroupDefinition {
   text GroupType
   text GroupID
}
class GroupMembers {
   text GroupID
   text GroupMemberID
}
class GroupTypes {
   text GroupType
}
class HamletLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   string LookupName
   text Name
}
class HoboGeneralTraffic {
   string CharacterID
}
class HogsmeadeMapLocations {
   real XPos
   real YPos
   real ZPos
   text IconName
   text MinimapIconName
   boolean FastTravel
   text LocationID
}
class HogwartsExpressSchedule {
   integer StartTime
   boolean Sunday
   boolean Monday
   boolean Tuesday
   boolean Wednesday
   boolean Thursday
   boolean Friday
   boolean Saturday
   string ScheduleName
}
class HogwartsMapIconTable {
   real OverrideLocationX
   real OverrideLocationY
   real OverrideLocationZ
   text IconName
   text Type
   text Region
   boolean ShowOnRegionTier
   text Name
}
class Houses {
   text DormLocationID
   text HouseID
}
class IdentityTypes {
   text TypeID
}
class InfirmaryDynamic {
   integer Priority
   text StudentID
}
class InventoryCapacity {
   integer InventoryCapacity
   integer SolvedSphinxPuzzles
}
class InventoryDynamic {
   text ItemID
   text Variation
   integer Count
   boolean Stolen
   boolean UniqueItem
   boolean KeepOnReset
   integer UpdateTime
   text CharacterID
   text HolderID
   integer SlotNumber
}
class InventoryHolderDefinition {
   int MultiSlotsPerItem
   integer LimitedSlots
   integer ReturnExcess
   integer MaxSlots
   text InventoryFullString
   text InventoryHolderID
}
class InventoryHolderSlotExpansions {
   integer SlotAmount
   text LockID
   text InventoryHolderID
}
class InventoryQuality {
   integer EInventoryQuality
   text EInventoryQualityNames
}
class InventorySlotDefinition {
   integer SlotCapacity
   text SlotLevel
}
class InvestigatableDynamic {
   integer Investigations
   text InvestigatableID
}
class ItemDefinition {
   text ItemType
   text ItemType2
   text RarityTier
   integer ItemLevel
   integer EconomyValue
   integer SellPrice
   boolean Inventoryable
   boolean Persistent
   boolean Giftable
   boolean Sellable
   boolean Dropable
   text SlotLevel
   text ItemUsagetype
   text ItemUsageObjectID
   boolean Consumable
   boolean TriggerAbilityOnConsume
   text LockID
   text OnUseLockID
   text PrerequisiteLockID
   text PrerequisiteLockID2
   boolean UsableFromInventory
   text UIDisplayMethod
   boolean UsableOnDiamond
   text StorageLocation
   text ItemID
}
class ItemKnowledgeCardMap {
   text KnowledgeCard1
   text KnowledgeCard2
   text KnowledgeCard3
   text ItemID
}
class ItemTypes {
   text ItemTypes
}
class ItemUsageTypes {
   text ItemUsageType
}
class ItemUseRestrictionDefinition {
   text RestrictionType
   text ItemID
}
class ItemUseRestrictionTypes {
   text RestrictionType
}
class ItemUsesAndSources {
   text Uses1
   text Uses2
   text Sources1
   text Sources2
   text Sources3
   text ItemID
}
class ItemsDynamic {
   text WorldObjectID
   integer EInteractiveState
   text LevelName
   real XPos
   real YPos
   real ZPos
   real ZRot
   boolean Stolen
   boolean IsUnique
   integer ItemCount
   text Variation
   integer ParentUID
   integer WorldObjectUID
}
class KnowledgeActions {
   real KnowledgePoints
   text EKnowledgeLevel
   text EKnowledgeApplicability
   boolean PlayerIsInteractor
   integer ExperiencePoints
   integer CompanionBondingPoints
   text EKnowledgeAction
}
class KnowledgeApplicability {
   text EKnowledgeApplicability
}
class KnowledgeCardPerks {
   text AbilityID
   text SubjectID
   text KnowledgeLevel
}
class KnowledgeCategories {
   text KnowledgeCategoryID
}
class KnowledgeDynamic {
   real KnowledgePoints
   text KnownExpert
   text RegistryID
}
class KnowledgeFactTypes {
   text TableID
   text SubjectColumnID
   text KnowledgeCategory
   text UI_Category
   text CustomQuery
   text ColumnID
}
class KnowledgeFacts {
   text EKnowledgeLevel
   text LockName
   text SubjectID
   text ColumnID
}
class KnowledgeHogwartsFacts {
   text HogwartsLore1
   text HogwartsLore2
   text HogwartsLore3
   text HogwartsLore4
   text HogwartsLore5
   text HogwartsLore6
   text HogwartsLore7
   text LocationID
}
class KnowledgeInvestigatable {
   real XPos
   real YPos
   real ZPos
   real ZRot
   string Name
}
class KnowledgeLevels {
   real KnowledgeLevelMaxPoints
   text EKnowledgeLevel
}
class KnowledgeLocationFacts {
   text RegionResource1
   text RegionResource2
   text RegionResource3
   text RegionResource4
   text RegionResource5
   text RegionResource6
   text RegionResource7
   text Hamlet1
   text Hamlet2
   text Hamlet3
   text Hamlet4
   text Hamlet5
   text Hamlet6
   text Hamlet7
   text LocationID
}
class KnowledgeLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class KnowledgeMiscFacts {
   text MiscLore1
   text MiscLore2
   text MiscLore3
   text MiscLore4
   text MiscLore5
   text ItemID
}
class KnowledgeSubjectTables {
   text DefinitionColumnID
   text DefinitionTableID
}
class KnowledgeSubjects {
   text SubjectCategory
   text AwardOnUnlock
   text SubjectID
}
class KnowledgeTutorialFacts {
   text Step1
   text Step2
   text Step3
   text Step4
   text Step5
   text Step6
   text Step7
   text Step8
   text TutorialID
}
class KnowledgeVendorFacts {
   text Vendor1
   text Vendor2
   text Vendor3
   text OpenTime
   text ShopID
}
class LocationNamedVolumes {
   text Code
   integer LocationIndex
   text VolumeName
   text LocationID
}
class Locations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text WorldID
   text TypeID
   text ParentLocationID
   real VolumeOriginX
   real VolumeOriginY
   real VolumeOriginZ
   real VolumeExtentX
   real VolumeExtentY
   real VolumeExtentZ
   real VolumeRotX
   real VolumeRotY
   real VolumeRotZ
   integer HouseAndGender
   text LocationID
}
class LockDefinition {
   text LockTypeID
   text LockMsg
   text LockID
}
class LockMessages {
   text LockMsg
}
class LockProgression {
   text LockID
   text ActionType
   text ActionData
}
class LockStates {
   text ELockStateName
   integer ELockStates
}
class LockTypes {
   integer ELockState0
   integer ELockState1
   text LockTypeID
}
class LockableComponentsDynamic {
   boolean Locked
   boolean ShowLock
   boolean PerceptibleWhenLocked
   integer LockDifficulty
   text ID
}
class LocksDynamic {
   integer ELockState
   text LockID
}
class LootCategories {
   text TypeID
   integer ContainerRollsLow
   integer ContainerRollsHigh
   string RollType
   text CategoryID
}
class LootCategoryTypes {
   text CategoryTypeID
}
class LootContainerContents {
   integer ContainerRandomWeight
   integer ContainerWeightAdjust
   integer ItemRollCount
   integer NPCRangeLow
   integer NPCRangeHigh
   text RequiredUnlock
   text Knowledge
   text KnowledgeLevel
   string GenerationType
   text LootCategoryID
   text ContainerID
}
class LootDropComponentDynamic {
   text LootGroup
   text UniqueID
}
class LootGenerationType {
   string GenerationType
}
class LootItemsDynamic {
   text ItemID
   boolean Looted
   integer ItemRandomWeight
   integer ItemAdjustedWeight
   text Variation
}
class LootRollTypes {
   string RollTypes
}
class LootTrackingDynamic {
   text LootCategoryID
   text ContainerID
   integer AdjustedWeight
}
class MailDynamic {
   text MailTextKey
   integer MailType
   integer AttachedContainerSize
   text AttachedContainerID
   text MissionID
   integer SentMinute
   integer ReadMinute
   text Sender
   integer State
   integer Noticed
   integer MissionCritical
   integer ShouldAutoPlay
   integer DisplayPriority
}
class MapGreaterRegions {
   text GreaterRegionName
}
class MapHogwartsLocations {
   text Region
   real LocationX
   real LocationY
   real LocationZ
   text Name
}
class MapHogwartsRegions {
   real LocationX
   real LocationY
   real LocationZ
   text IconName
   string FocusLocation
   string RequiredLock1
   text Name
}
class MapLocationDataDynamic {
   integer State
   text MapLocationID
}
class MapLocationHints {
   unknown GreaterRegion
   boolean FavorODCFoundPath
   boolean DisableTargetHeightAdjust
   text Name
}
class MapMarkup {
   text RegionType
   boolean ShowBanner
   text LocationID
}
class MiscDataDynamic {
   text DataValue
   text DataOwner
   text DataName
}
class MiscLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   string Owner
   text Name
}
class MissionContainerDynamic {
   text MissionID
   text ContainerID
   integer ContainerSize
   text ItemID
   integer ItemQuantity
   text ItemVariation
}
class MissionDefinition {
   text ParentMissionID
   text MissionLineID
   text MissionTitleTextKey
   text MissionSummaryTextKey
   text MissionLevel
   text SuggestedMissionLevel
   text MissionPrereqLockID1
   text MissionPrereqLockID2
   text ProgressLockID
   text AchievementID
   text KnowledgeSubject
   boolean Discoverable
   boolean DisableAbandonment
   boolean ProcessDuringExclusiveMissions
   boolean AlwaysReset
   boolean CompleteChildrenWhenDone
   text MissionAvailableTextKey
   text MissionActiveTextKey
   text MissionID
}
class MissionDynamic {
   text MissionID
   text Type
   text Text1
   text Text2
   text Text3
   text Text4
   text Text5
   text Text6
   integer Integer1
   integer Integer2
   integer Integer3
   integer Integer4
   integer Integer5
   integer Integer6
   integer Integer7
}
class MissionKnowledgeSubjects {
   text KnowledgeSubject
}
class MissionLighthouseGoals {
   text LighthouseGoalID
}
class MissionLighthouseSubgoals {
   text SubgoalOverride
   text LighthouseGoalID
   integer SubgoalOrder
   text MissionID
}
class MissionLines {
   text InterfaceText
   integer InterfaceOrder
   text MissionLineID
}
class MissionNamedGroups {
   int HideOnPlatform
   text GroupName
   text CharacterID
}
class MissionRewardTypes {
   text TypeID
}
class MissionRewardUICategories {
   text UICategoryID
}
class MissionRewards {
   text TypeID
   text RewardID
   text Size
   integer Quantity
   boolean Hidden
   text UICategoryID
   text RewardNickname
   text MissionID
   integer RewardIndex
}
class MissionStatuses {
   text InterfaceText
   integer InterfaceOrder
   text MissionStatusID
}
class MissionSteps {
   text TaskTypeID
   integer Flags
   text StepNickname
   text GotoStepNickname
   text Keyword1
   text Keyword2
   text Keyword3
   text Keyword4
   text Keyword5
   text Keyword6
   text Keyword7
   text Keyword8
   text Keyword9
   text Keyword10
   text Keyword11
   text StepJournalTextKey
   text StepObjectiveTextKey
   text StepFailTextKey
   text StepFailWarning
   integer TaskUID
   text MissionID
   real Step
}
class MissionTaskKeywordType {
   text TaskKeywordTypeID
}
class MissionTaskTypes {
   text Keyword1Type
   text Keyword2Type
   text Keyword3Type
   text Keyword4Type
   text Keyword5Type
   text Keyword6Type
   text Keyword7Type
   text Keyword8Type
   text Keyword9Type
   text Keyword10Type
   text Keyword11Type
   boolean StepEvaluationIgnores
   boolean IsAction
   text TaskTypeID
}
class NPCLevelScaling {
   real Health
   integer MinLevel
   integer MaxLevel
   integer MinDeviation
   integer MaxDeviation
   integer LevelBoost
   integer BoostFallOff
   integer FallOffStart
   integer FallOffEnd
   text HealthModLevel
   text DamageModLevel
   text CharacterID
}
class NPCMultiplierCurveData {
   real HealthValueStory
   real DamageValueStory
   real NPCDamageValueStory
   real HealthValueEasy
   real DamageValueEasy
   real NPCDamageValueEasy
   real HealthValue
   real DamageValue
   real NPCDamageValue
   real HealthValueHard
   real DamageValueHard
   real NPCDamageValueHard
   integer Level
}
class NPCMultiplierData {
   real Health
   real Damage
   text Level
}
class NPCSpellLoadouts {
   text DefaultSpell
   text CombatSpell1
   text CombatSpell2
   text CombatSpell3
   text CombatSpell4
   text CombatSpell5
   text CombatSpell6
   text Name
}
class NamedCreatureDefinition {
   integer CreatureUID
   text TypeID
   text CreatureName
   boolean IsLocalizedName
   boolean IsUncapturable
   boolean IsGenderMale
   boolean IsMount
   boolean CanRename
   boolean CanReturnToWild
   text ColorVariation
   double ScaleVariation
   text NurturingSpaceID
   real Happiness
   boolean SimulationEnabled
   text NamedCreatureID
}
class Noise {
   text Intensity
   real Radius
   text Noise
}
class NurturingCreatureDynamic {
   text TypeID
   text CreatureName
   boolean IsLocalizedName
   boolean IsUncapturable
   boolean IsGenderMale
   boolean IsMount
   boolean CanRename
   boolean CanReturnToWild
   text ColorVariation
   double ScaleVariation
   text NurturingSpaceID
   integer MotherUID
   integer FatherUID
   integer BreedingGeneration
   integer BirthDateTime
   real Happiness
   integer PregnancyState
   integer PregnancyStartDateTime
   integer IncubationStartDateTime
   integer PenUID
   boolean ProducingByproduct
   integer LastUpdateDateTime
   integer PlacedInNurturingSpaceDateTime
   boolean NeedMet_Fed
   boolean NeedMet_Interaction
   real ByproductCooldownProgress
   boolean SimulationEnabled
   boolean EnableSimulationWhenFirstSpawned
   integer CreatureUID
}
class NurturingSpaceDefinition {
   integer MaxNumCreatures
   integer MaxNumSpecies
   integer MaxCreatureCompletedYearForCapture
   text NurturingSpaceID
}
class ObjectAndOwner {
   string Owner
   string Name
}
class ObjectLocations {
   text ObjectID
   text LocationID
}
class OutfitItemTypes {
   real OrderID
   boolean CanBeEmpty
   text SocketName
   text OutfitItemTypeID
}
class OutfitTypes {
   text OutfitTypeID
}
class PerkCategories {
   text CategoryType
}
class PerkDefinition {
   text PerkType
   integer LevelRequirement
   integer UIColumn
   integer UIRow
   text AbilityID
   text LockRequirement
   text LockRequirement2
   text PerkID
}
class PerkDynamic {
   integer Level
   text PerkID
}
class PerkStates {
   text EPerkStateName
   integer EPerkStates
}
class PerkTypes {
   text PerkTypeID
}
class PlantDefinition {
   integer Tier
   text Plant_LockID
   text Plant_Product
   text PlotSize
   text SeasonID
   integer SortingIndex
   integer GrowthTimeSec
   boolean IsMultiHarvestable
   integer RegrowthTimeSec
   integer Yield_Planted
   integer Yield_Foraged
   text PlantID
}
class PlantPersistenceDynamic {
   integer ParentUID
   integer ObjectID
   integer EInteractiveState
}
class PlantSizes {
   integer PlantSizeIndex
   text PlantSizeID
}
class PlantSources {
   text PlantSource
}
class PlantUses {
   text PlantUse
}
class PlayerHealthLevelMap {
   integer PlayerHealth
   integer PlayerLevel
}
class PlayerStatsDynamic {
   text ActivityValue
   integer ElapsedGameTime
   text ActivityType
   text ActivityName
   text CompanionName
}
class PlotDefinition {
   text PlotSize
   text PlotID
}
class PlotDynamic {
   integer StationUID
   text PlotID
   text PlantID
   text FertilizedWith
   boolean FertilizedByPlayer
   integer GrowthState
   integer LastUpdateDateTime
   double ProgressAtLastUpdate
   integer PlotUID
}
class PointsOfInterest {
   real PositionX
   real PositionY
   real PositionZ
   real DiscoverDistance
   string State
   string PointOfInterestID
}
class PointsOfInterestDynamic {
   string PointOfInterestID
}
class PostDeathCleanUpEffects {
   text CleanUpEffect
}
class PostDeathCleanUpModes {
   text CleanUpModes
}
class PostDeathParams {
   integer BatchSize
   integer MaxAllowedNPCs
   integer MinAllowedNPCs
   double TimeBetweenBatches
   double TimerModeDelay
   text CleanUpEffect
   text CleanUpMode
   text SortingMode
   text LevelName
}
class PostDeathSortingModes {
   text SortingMode
}
class PotionDefinition {
   text PotionTypeID
   text LockID
   text UICategory
   integer SortingIndex
   text Ingredient1
   integer Quantity1
   text Ingredient2
   integer Quantity2
   text Ingredient3
   integer Quantity3
   text Ingredient4
   integer Quantity4
   text Ingredient5
   integer Quantity5
   text Ingredient6
   integer Quantity6
   integer TimeToBrewSec
   integer Yield
   unknown ProductID
   text PotionID
}
class PotionTypes {
   text PotionTypeID
}
class PotionUnitTypes {
   text UnitID
}
class Potions made from Creatures {
   text PotionID
}
class Potions made from Plants {
   text PotionID
}
class ProductIDs {
   text PS5
   text PS4
   text XBox
   text Steam
   text Switch
   text Epic
   text EpicOfferIDs
   text Hydra
   integer bPurchasable
   text Title
   text Description
   text Notes
   string ItemName
}
class RPGAbilityDurationDefinition {
   real Duration
   text Units
   text UpgradeAbilityTag
   real UpgradeDuration
   text UpgradeUnits
   text AbilityID
}
class RPGAbilityDynamic {
   string ActorID
   text AssetPath
   real CurrentLifeTime
   real MaxLifeTime
   boolean ResetOnSleep
   string AbilityID
}
class RPGItemAbilityDynamic {
   text DurationType
   real CurrentLifeTime
   real MaxLifeTime
   bigint StartTimeStamp
   bigint EndTimeStamp
   text Variation
   text ActorID
   text AbilityName
}
class RPGPermaAbilityDynamic {
   text ActorID
   text AbilityName
}
class RPGSystemCooldownDefinition {
   real CooldownTime
   string CooldownName
}
class RPGSystemCooldowns {
   string CooldownGroup
   string AbilityName
}
class RarityTierType {
   real TypeID
}
class Registry {
   text SubtypeID
   text RegistryID
}
class RegistryTypes {
   text DynamicTable
   boolean AllowDynamicSpawn
   boolean AllowBeacon
   boolean AllowInObjectState
   boolean AllowInOwnership
   text PersistenceTable
   text RegistryTypeID
}
class RichPaperDefinition {
   string RichPaperTypeID
   text ImageName
   text HeaderTextKey
   text BodyTextKey
   text FooterTextKey
   text RichPaperID
}
class RichPaperDynamic {
   text RichPaperID
}
class RichPaperTypes {
   text RichPaperTypeID
}
class RuinLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   string Name
}
class SancFeedingStationDynamic {
   text LevelName
   integer AvailableFeed
   integer UID
}
class SanctuaryAreas {
   text ConjurationContext
   text AreaID
}
class SanctuaryBiomeDefinition {
   text LevelSubstring
   text NurturingSpaceID
   text BiomeID
}
class SanctuaryBiomeDynamic {
   integer NumFeedingStations
   text BiomeID
}
class SanctuaryExpansionDefinition {
   text ExpansionLockID
   text AreaID
   integer ExpansionIndex
}
class SanctuaryHousekeepingDefinition {
   double SpawnNumPerInterval
   integer MaxNumPerZone
   integer MinIntervalsToRespawn
   text Type
}
class SanctuaryHousekeepingDynamic {
   text Type
   text ZoneID
   boolean IsAlive
   integer LastDestroyedIntervalIndex
   text LockID
   text LockID2
   integer ObjectUID
}
class SanctuaryHousekeepingZones {
   text ZoneID
}
class SanctuaryInitialCustomizationChoices {
   integer StructureIdentityIndex
   text StructureColor
   integer LightingIdentityIndex
   text DressingLock
   text Name
}
class SanctuaryItemGeneratorData {
   text LootCategoryID
   integer GenerationTimeSec
   text ItemGenerator
}
class SanctuaryItemGeneratorDynamic {
   text TransfigObjectCategory
   text ItemHeld
   integer ItemQuantity
   integer GenerationCompleteTime
   integer ItemGeneratorUID
}
class SanctuaryNamedChestDynamic {
   text CustomName
   integer ObjectUID
}
class SceneRigCompletedDynamic {
   integer Completed
   text Key
}
class ScheduleDynamic {
   text ActiveKey
   text CharacterID
}
class ScheduleEntryTypes {
   string TypeID
}
class Schedule_Azkaban {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cairn_Dungeon_2 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cairn_Dungeon_20 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cairn_Dungeon_21 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cairn_Dungeon_3 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cairn_Dungeon_8 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Castle_Dungeon_1 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Castle_Dungeon_10 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Castle_Dungeon_11 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Castle_Dungeon_15 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Castle_Dungeon_19 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Castle_Dungeon_22 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cav_Dungeon_01 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cav_Dungeon_02 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cav_Dungeon_05 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cav_Dungeon_08 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cav_Dungeon_12 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cavern_Dungeon_10 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cavern_Dungeon_19 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cavern_Dungeon_24 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cavern_Dungeon_26 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Cavern_Dungeon_33 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Cavern_Dungeon_34 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_DeathHallows_Dungeon {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Default {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Empty {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_GeneratedDefaults {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text Filter
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_GeneratedLocationIds {
   text LocationID
}
class Schedule_GeneratedLocations {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_GobMine_Dungeon_07 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_GobMine_Dungeon_13 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Gobmine_Dungeon_01 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Gobmine_Dungeon_06 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Gobmine_Dungeon_11 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Gobmine_Dungeon_12 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_HM_ExtortionistHideout {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_HOG_Dungeon_01 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_HauntedShop_Dungeon_02 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_HauntedShop_Dungeon_03 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Hogsmeade_Dungeon_02 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Hogwarts_Dungeon_02 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Hogwarts_Dungeon_Evil {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Intro {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Marketing {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Overland {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_Pensieve_Tomb_2 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_PoacherHideout {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_RootLevel {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text CharacterID
   text ActivityID
   integer OverrideStartTime
   text ScheduleKeys
}
class Schedule_SancStudy {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_Sanctum_Dungeon_Cavern2 {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_SpawnOnly {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_ThievesHideout {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class Schedule_ZZS_TrollFight {
   integer Priority
   text OverrideLocationID
   text PropTypeID
   integer OverrideEndTime
   text EntryTypeID
   text ScheduleKeys
   text Filter
   text CharacterID
   text ActivityID
   integer OverrideStartTime
}
class SchedulesForLevels {
   text ScheduleName
   string WorldKeys
   boolean WantHobos
   real BV_MinX
   real BV_MinY
   real BV_MinZ
   real BV_MaxX
   real BV_MaxY
   real BV_MaxZ
   text LevelName
}
class Seasons {
   text SeasonID
}
class SeatFillerSchedule {
   text LocationID
   integer StartTime
   integer EndTime
   text SubtypeID
   text Look
   text GenderID
   text HouseID
   integer Count
   text ActivityTypeID
   integer FillDistance
   integer ActivateWhenStreamed
   text ScheduleKey
}
class SecretFactsDefinition {
   text KeyID
   text SubjectID
   text ColumnID
}
class SkeletonTypes {
   text SkeletonTypeID
}
class SocialActionDefinition {
   text SocialActionTypeID
   integer SocialCapitalValue
   integer TargetSCMod
   integer WitnessSCMod
   integer HearsaySCMod
   integer SCDecayPercent
   integer Lifetime
   integer MaxPropagationCount
   text MinPropagationSCStatus
   integer Priority
   integer HousePoints
   text SocialActionID
}
class SocialActionDynamic {
   real ExpirationTime
   text LocationID
   integer SocialCapitalImpact
   boolean Squelched
   integer Reach
   text SocialActionID
   real ActionTime
   text ActionData
   text TargetCharacterID
}
class SocialActionObserverTypes {
   text ObserverTypeID
}
class SocialActionSemantics {
   integer Value
   text SocialActionID
   text SocialSemanticID
}
class SocialActionType {
   text SocialActionTypeID
}
class SocialCapitalStatuses {
   integer Threshold
   text SocialCapitalStatusID
}
class SocialConnectionStatuses {
   integer SocialCapitalBoost
   text SocialConnectionID
}
class SocialEconomicStatuses {
   text SocioEcoStatusID
}
class SocialHeritageStatuses {
   text SocialHeritageStatusID
}
class SocialInteractionData {
   text InteractionType
   integer DisplayOrder
   text IsCompanion
   text Stranger
   text Hate
   text Dislike
   text Indifferent
   text Familiar
   text Cordial
   text Friendly
   text Companion
   text RequiredMission
   text RequiredLock
   text CharacterType
   text CharacterID
   text InteractionLineID
}
class SocialInteractionDisplayStatuses {
   text SocialInteractionDisplayStatusID
}
class SocialInteractionTypes {
   text SocialInteractionTypeID
}
class SocialSemanticTypes {
   text SocialSemanticTypeID
}
class SocialSemantics {
   text SocialSemanticTypeID
   text SocialSemanticID
}
class SocialStationActionChoices {
   text PropType
   text CurrentAction
   integer OccupiedConnections
   integer NumConnectionsReqd
   text AvailableAction
   integer UseConnection
   integer UseConnectionAsSet
   integer TargetConnections
   text ActivityTypeID
   integer CurrentActionMustBeActive
}
class SpawnGroupDefinition {
   integer MinCount
   integer MaxCount
   text SpawnDiscoveryType
   boolean ForceSpawnOnGround
   boolean SpawnOnNavMesh
   boolean IsPersistent
   real SpawnProbability
   real SpawnDistanceFromAvatar
   real SelectionProbability
   integer RequiredPlayerLevel
   text RequiredProgressLockID
   text RegistryID
   text SpawnID
   integer SelectionGrouping
}
class SpawnGroupEconomy {
   int SpawnCount
   boolean ForceSpawnOnGround
   boolean IsPersistent
   real SpawnWeight
   text GroupName
   text SpawnID
}
class SpawnLocationTypes {
   text TypeName
}
class SpawnRestrictionCategories {
   unknown CategoryName
}
class SpawnRestrictionTypes {
   text RestrictionCategory
   text DataType
   text RestrictionName
}
class SpawnRestrictions {
   text Value
   text HouseAndGender
   text LockID
   text StatID
   integer StatValue
   text Name
   text Type
}
class SpellCategories {
   text TypeID
}
class SpellDefinition {
   real Range
   real CooldownTime
   real NonCombatCooldownMultiplier
   real DamageObject
   real DamageCharacter
   real PhysicsImpulseSuccess
   real PhysicsImpulseFailed
   text ImpactType
   text SizeLimit
   boolean AllowNonObjectInfoActors
   real Duration
   real DurationCharacter
   real DurationCreature
   real DurationPlayer
   real ChargeTime
   real ChargedMaxTime
   real ChannelingMinTime
   boolean Animate
   boolean Inanimate
   boolean Plant
   boolean Dead
   boolean Water
   boolean UpgradedMechanics
   boolean PlayObjectImpactEffects
   integer LimitedCountObject
   integer LimitedCountCharacter
   boolean PlayerShieldBreaker
   text EnemyShieldBreaker
   text CastNoise
   text ImpactNoise
   real ProjectileSpeed
   real ProjectileGravity
   boolean BeastCapture
   text SpellTypeID
   text Upgrade
}
class SpellImpactTypes {
   text EImpactTypesName
}
class SpellKnowledge {
   text SpellCategory
   text SpellIdentity
   text CurriculumAssociation
   boolean AllowInUI
   boolean AllowForCompanions
   unknown KnowledgeGain
   text UpgradeID0
   text Lock
   boolean NurtureOnly
   text SpellTypeID
}
class SpellMappingForLoadouts {
   text SocialSemantic
   text SpellID
}
class SpellObjectPropertyTypes {
   text EObjectPropertyTypeName
}
class SpellSizes {
   text EObjectSizeClassName
}
class SpellUpgradeAttributes {
   text SpellUpgradeAttribute
}
class SpellUpgrades {
   text SpellUpgrade
}
class SpellsDynamic {
   text Spell0
   text Spell1
   text Spell2
   text Spell3
   text Spell4
   text Spell5
   text Spell6
   text Spell7
   text Spell8
   integer LoadoutIndex
}
class SphinxPuzzleDefinition {
   text SphinxPuzzleID
}
class SphinxPuzzleDynamic {
   integer EInteractiveState
   text SphinxPuzzleGUID
}
class SphinxPuzzleInstance {
   text SphinxPuzzleTypeID
   text PuzzleName
   text WorldName
   text LevelName
   real XPos
   real YPos
   real ZPos
   real ZRot
   real LevelXPos
   real LevelYPos
   real OffsetX
   real OffsetY
   text SphinxPuzzleGUID
}
class SphinxPuzzleLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class StationCollisionType {
   text CollisionTypeID
}
class StationPropClasses {
   text PropClassID
}
class StationPropTypes {
   text PropClassID
   text PropTypeID
}
class StationSiteVicinityScale {
   real ScaleX
   real ScaleY
   real ScaleZ
   text LocationID
}
class StatsDynamic {
   integer Value
   boolean Transient
   text StatID
}
class StoryGraphPersistenceDynamic {
   text Key
   text NodeName
   integer IsActive
   text ActivationSource
}
class StudentList {
   text RegistryID
}
class SubjectDefinition {
   text SubjectTypeID
   text Professor
   text SubjectID
}
class SubjectOfTheDayKnowledgeCards {
   text LockID
   text SubjectID
   text KnowledgeCard
}
class SubjectTypes {
   text SubjectTypeID
}
class SublevelWorld {
   text World
   text Sublevel
}
class SubtypeInteraction {
   text InteractorSubtype
   text InteracteeSubtype
   text Interaction
   text InteractionAfraid
   integer Priority
}
class Subtypes {
   text RegistryTypeID
   boolean Customizable
   text SubtypeID
}
class TabooItemList {
   string ItemID
}
class TentLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class TerrainAnchorGroups {
   numeric DensityPerSquareMeter
   numeric MinimumDistance
   string Mesh1
   string Mesh2
   string Mesh3
   string Mesh4
   string Mesh5
   string Mesh6
   string Mesh7
   string Mesh8
   string GroupName
}
class TerrainAnchorSpawnGroups {
   string Group1Name
   string Group2Name
   string Group3Name
   string Group4Name
   string SpawnGroup
}
class TerrainAnchors {
   string SpawnGroup
   numeric Radius
   numeric MinObjectRadius
   boolean IsAreaFixed
   string AnchorType
}
class TileForegeableSpawning {
   text Tile
   text Category
   text SpawnID
   int Density
   int LocationAmount
   boolean IsPersistent
}
class TransfigurationCategoryList
class TransfigurationClasses {
   integer IsPrefab
   integer SupportsTransformation
   text TransformationStyle
   integer SupportsVanishment
   text VanishmentStyle
   integer SupportsLevitation
   integer SupportsColovaria
   integer SupportsScaling
   integer SupportsRotation
   text StreamingPriority
   text TransfigSlotTypeID
   integer RemoveFoliage
   integer UseSurfacePlacement
   text ProtectedInMissions
   text Class
}
class TransfigurationColors {
   text Color
}
class TransfigurationDynamic {
   text TypeID
   text OriginalTypeID
   text LevelName
   double LocX
   double LocY
   double LocZ
   double RotX
   double RotY
   double RotZ
   double ScaleX
   double ScaleY
   double ScaleZ
   integer IsConjured
   text ColorID
   integer ObjectUID
}
class TransfigurationExpansionDynamic {
   text ExpansionLockID
   text ExpandedCategory
   integer ObjectUID
}
class TransfigurationGroups {
   text Groupname
}
class TransfigurationNamedObjectsDynamic {
   integer ObjectUID
   text Name
}
class TransfigurationObjectGroups {
   unknown Groupname
   text Category
}
class TransfigurationObjectLocks {
   text LockID
   text ObjectID
}
class TransfigurationObjectStatsCategories {
   text ObjectCategory
   text StatsCategory
}
class TransfigurationObjects {
   text ConjurationCategory
   text ConjurationCategory2
   text Snapping
   text SocketCategory
   text Class
   double SmallScaleOverride
   double LargeScaleOverride
   integer SortingIndex
   integer BudgetCost
   text TransformationGroup
   text Item1
   text Item2
   text Item3
   text Item4
   text Item5
   text Item6
   text Item7
   text Item8
   text Resource1_ID
   integer Resource1_Required
   text Resource2_ID
   integer Resource2_Required
   text Resource3_ID
   integer Resource3_Required
   text Resource4_ID
   integer Resource4_Required
   text Resource5_ID
   integer Resource5_Required
   text Category
}
class TransfigurationSlotPoolExpansions {
   integer SlotAmount
   text LockID
   text SlotID
}
class TransfigurationSlotPools {
   integer PoolStartAmount
   text TransfigSlotID
}
class TransfigurationSnapping {
   text Snapping
}
class TransfigurationSocketCategories {
   text Category
}
class TransfigurationStatsCategories {
   text ConjurationCategory
   text StatsCategory
}
class TransformationGroups {
   text GroupID
}
class TransformationOverlandResults {
   text Transformation1
   real Weight1
   text Transformation2
   real Weight2
   text Transformation3
   real Weight3
   text Transformation4
   real Weight4
   text ResultCategory
}
class TransformationOverlandTargets {
   text ResultCategory1
   real Weight1
   text ResultCategory2
   real Weight2
   text ResultCategory3
   real Weight3
   text ResultCategory4
   real Weight4
   text Category
}
class TransformationStreamingPriority {
   text Priority
}
class TransformationStyles {
   text Style
}
class TriggeredEffectTypes {
   string EffectType
}
class TriggeredEffects {
   text EffectID
   string EffectType
   numeric Units
   numeric Percentage
   string Duration
   text LinkedEffect
   text EffectSourceID
}
class TutorialQueuePersistenceDynamic {
   text Name
   text Alias
   integer Step
   integer QueueIndex
}
class UDSAlternativeMissionNames {
   string OriginalName
   string AlternativeName
}
class UDSAlternativeTaskNames {
   string NewParent
   string OriginalName
   string AlternativeName
}
class UIActionGroupDynamic {
   text Spell_North
   text InventoryItem_North
   text Spell_East
   text InventoryItem_East
   text Spell_South
   text InventoryItem_South
   text Spell_West
   text InventoryItem_West
   integer GroupID
}
class UIActionItem {
   text SpellID
   text InventoryItemID
   text ItemVariation
   text StorageLocation
   integer ItemID
}
class UIActionModes {
   text ModeID
}
class UIInputActions {
   string ActionID
}
class UIKeyBindingsDynamic {
   string PCController
   string PCKeyboard
   string XboxOne
   string PS4
   string Switch
   string PS5
   string XSX
   string InputKey
}
class UIKnowledgeCategories {
   text CategoryID
}
class UILoadingScreenBackgrounds {
   string Area
   string SpecificLevelName
   string UnlockedAfterMission
   string LockedAfterMission
   string BackgroundID
}
class UILoadingScreenTips {
   string MainSystem
   string SubSystem
   string Area
   string UnlockedAfterMission
   string LockedAfterMission
   string TipID
}
class UIQuickActionsDynamic {
   integer LayoutID
   integer GroupIndex
   text ButtonID
   integer MacroSlotIndex
   text SpellID
   text InventoryItemID
   text ItemVariation
   text StorageLocation
   integer ActionBarID
}
class UITwitchActions {
   text Spell
   text ItemID
   text ControllerButton
}
class UIWorldActions {
   integer FaceButtonActionGroup
   integer DPadGroup1
   integer DPadGroup2
   integer DPadGroup3
   integer DPadGroup4
   text StorageLocation
   integer AllowEditing
   integer HonorSpellKnowledge
   text DefaultActionMode
   text WorldName
}
class UnresolvedDoorStatesDynamic {
   text State
   boolean LockVisible
   boolean PlaySoundsAndEffects
   text DoorName
}
class VanishmentStyles {
   text Style
}
class VaultLocations {
   real XPos
   real YPos
   real ZPos
   real ZRot
   text Name
}
class VendorConversationsDynamic {
   text VendorID
}
class VendorStocks {
   text VendorLocationID
   integer Weight
   integer MinItems
   integer WeightAdjustment
   text LockID
   text VendorID
   text ContainerID
}
class VendorStocksDynamic {
   string VendorID
   text ContainerID
   integer AdjustedWeight
}
class VendorUnavailableStock {
   text Lock
   text TextKey
   text VendorID
   text IconAssetKey
}
class VirtualContainerContents {
   text Variation
   integer ItemQuantity
   integer ItemQuantityHigh
   integer ItemRandomWeight
   integer ItemWeightAdjust
   boolean UniqueItem
   boolean ShowInCurriculumRewards
   text VContainerID
   text ItemID
   text LockID
   text ContainerID
}
class VirtualContainerList {
   text SubtypeID
   text VContainerID
}
class VirtualContainerTypes {
   text TypeID
}
class WorldAdjustments {
   text Name
}
class WorldEventsDynamic {
   string WorldEventName
   string LocationGuid
}
class WorldEventsPersistenceDynamic {
   string WorldEventName
   integer Stage
   boolean Completed
}
class WorldObjectDefinition {
   text WorldObjectID
}
class WorldObjectDynamic {
   text WorldObjectID
   integer ParentUID
   integer EInteractiveState
   text ObjectName
   text LevelName
   real XPos
   real YPos
   real ZPos
   real ZRot
   integer WorldObjectUID
}
class WorldRegionAdjustments {
   integer Min
   integer Max
   text Region
   text Adjustment
}
class WorldRegions {
   text Name
}
class sqlite_master {
   text type
   text name
   text tbl_name
   int rootpage
   text sql
}
class sqlite_sequence {
   unknown name
   unknown seq
}

AchievementChallenges  -->  AchievementChallengeCategory : AchievementCategory
AchievementChallenges  -->  ExperienceActions : ProgressExperience:ExperienceAction
AchievementCriteria  -->  AchievementDefinition : AchievementID
AchievementCriteria  -->  KnowledgeActions : KnowledgeAction:EKnowledgeAction
AchievementCriteria  -->  KnowledgeCategories : KnowledgeCategory:KnowledgeCategoryID
AchievementCriteria  -->  LockDefinition : PrerequisiteLockID:LockID
AchievementCriteria  -->  LockDefinition : AwardOnUnlock:LockID
AchievementDefinition  -->  AchievementTypes : AchievementType
AchievementRewards  -->  AchievementDefinition : AchievementID
AchievementRewards  -->  AchievementRewardCategory : RewardCategory
AchievementRewards  -->  AchievementRewardTypes : RewardType
AcknowledgementDynamic  -->  AcknowledgementRules : AcknowledgementID:VOEventID
AcknowledgementMissionDisablesVO  -->  MissionDefinition : MissionID
AcknowledgementMissionStats  -->  MissionDefinition : MissionID
AcknowledgementRules  -->  AcknowledgementNPCType : NPCType
ActivityCriticalResult  -->  Houses : ProfessorHouse:HouseID
ActivityCriticalResult  -->  SubjectDefinition : SubjectID
ActivityDefinition  -->  ActivityRecurrenceTypes : ActivityRecurrenceTypeID
ActivityDefinition  -->  ActivityTypes : ActivityTypeID
ActivityDefinition  -->  Locations : LocationID
ActivityDefinition  -->  Seasons : SeasonID
ActivityDefinition  -->  SubjectDefinition : SubjectID
ActivityTypes  -->  OutfitTypes : OutfitTypeID
ActorDefinition  -->  CharacterEmoteVoices : EmoteVoiceID
ActorDefinition  -->  CharacterVoices : AdditionalVoiceID:VoiceID
ActorDefinition  -->  Genders : GenderID
ActorDefinition  -->  Registry : RegistryID
ActorDefinition  -->  SkeletonTypes : SkeletonTypeID
AmbientCreatureDefinition  -->  CreatureDefinition : CreatureID
AmbientCreatureGroupDefinition  -->  AmbientCreatureDefinition : CreatureID
AmbientCreatureGroupDefinition  -->  AmbientCreatureFrequencyDefinition : Frequency
AmbientCreatureGroupDefinition  -->  AmbientCreatureGroup : GroupID
AvatarFullBodyPresetsDynamic  -->  Registry : RegistryId:RegistryID
BeaconDataDynamic  -->  Locations : LocationID
BroomRaceTimesDynamic  -->  BroomRaceDefinition : RaceName
BuffAttributeType  -->  BuffActionType : ActionID
BuffAttributeType  -->  BuffFocusType : FocusID
CharacterDefinition  -->  CharacterDefinition : CopyScheduleFromCharacterID:CharacterID
CharacterDefinition  -->  Houses : HouseID
CharacterDefinition  -->  LockDefinition : CompanionLock:LockID
CharacterDefinition  -->  LootCategories : LootDrop:CategoryID
CharacterDefinition  -->  Registry : CharacterID:RegistryID
CharacterDefinition  -->  Seasons : BirthdaySeason:SeasonID
CharacterDefinition  -->  SocialEconomicStatuses : SocioEconomicStatus:SocioEcoStatusID
CharacterDefinition  -->  SocialHeritageStatuses : SocialHeritage:SocialHeritageStatusID
CharacterDefinition  -->  SocialSemantics : FactionID:SocialSemanticID
CharacterDefinition  -->  SocialSemantics : IdentityID:SocialSemanticID
CharacterLoadoutsDynamic  -->  Registry : Name:RegistryID
CharacterLoadoutsDynamic  -->  SpellKnowledge : CombatSpell1:SpellTypeID
CharacterLoadoutsDynamic  -->  SpellKnowledge : CombatSpell6:SpellTypeID
CharacterLoadoutsDynamic  -->  SpellKnowledge : CombatSpell3:SpellTypeID
CharacterLoadoutsDynamic  -->  SpellKnowledge : CombatSpell5:SpellTypeID
CharacterLoadoutsDynamic  -->  SpellKnowledge : CombatSpell4:SpellTypeID
CharacterLoadoutsDynamic  -->  SpellKnowledge : DefaultSpell:SpellTypeID
CharacterLoadoutsDynamic  -->  SpellKnowledge : CombatSpell2:SpellTypeID
CharacterLookOverrideDynamic  -->  Registry : RegistryID
CharacterLookOverrideDynamic  -->  Registry : OverrideRegistryID:RegistryID
CharacterOutfitTypes  -->  OutfitTypes : OutfitTypeID
CharacterOutfitTypes  -->  Subtypes : SubtypeID
CharactersDynamic  -->  CharacterDefinition : CharacterID
CharactersDynamic  -->  SocialSemantics : ExtortionIdentity:SocialSemanticID
CharactersDynamic  -->  SocialSemantics : FavorIdentity:SocialSemanticID
CharactersDynamic  -->  SocialSemantics : Identity2:SocialSemanticID
CharactersDynamic  -->  SocialSemantics : Identity3:SocialSemanticID
CollectionActions  -->  CollectionItems : ItemID
CollectionActions  -->  CollectionStates : CollectionState
CollectionActions  -->  KnowledgeActions : KnowledgeAction:EKnowledgeAction
CollectionActions  -->  LockDefinition : LockID
CollectionItems  -->  CollectionCategories : CategoryID
CollectionItems  -->  CollectionSubcategories : SubcategoryID
CollectionItems  -->  LockDefinition : AOCLock:LockID
CompanionStatsTriggersDynamic  -->  CompanionStatsConditionDefinition : Condition:ConditionID
CompanionStatsTriggersDynamic  -->  CompanionStatsTriggerTypes : TriggerType:Type
CompanionStatsTriggersDynamic  -->  StatsDynamic : StatID
ConjurationCategory  -->  ConjurationCategory : ParentCategory:ConjurationCategory
ConjurationContextDefinition  -->  ConjurationCategory : ConjurationCategory
ConjurationContextDefinition  -->  ConjurationContext : ConjurationContext
ConversationDynamic  -->  CharacterDefinition : CharacterID
ConversationExclusiveDynamic  -->  CharacterDefinition : CharacterID
ConversationExclusiveDynamic  -->  MissionDefinition : RegisteredByMission:MissionID
CreatureAttributeFacts  -->  CreatureDefinition : CreatureID
CreatureColorVariationBreeding  -->  CreatureColorVariation : ChildVariation:ColorVariation
CreatureColorVariationBreeding  -->  CreatureColorVariation : ParentVariation2:ColorVariation
CreatureColorVariationBreeding  -->  CreatureColorVariation : ParentVariation1:ColorVariation
CreatureColorVariationDefinition  -->  CreatureColorVariation : ColorVariation
CreatureColorVariationDefinition  -->  CreatureDefinition : AdultID:CreatureID
CreatureDefinition  -->  AchievementDefinition : AchievementForCapturing:AchievementID
CreatureDefinition  -->  CreatureDefinition : Conflict2:CreatureID
CreatureDefinition  -->  CreatureDefinition : Conflict1:CreatureID
CreatureDefinition  -->  CurriculumYear : CompletedYearForCapture:Year
CreatureDefinition  -->  ItemDefinition : ByProduct:ItemID
CreatureDefinition  -->  Registry : PreferredToy:RegistryID
CreatureDefinition  -->  Registry : CreatureID:RegistryID
CreatureDefinitionMap  -->  CreatureDefinition : EnemyClass:CreatureID
CreatureDefinitionMap  -->  Registry : RegistryID
CreatureFamilies  -->  CreatureDefinition : EggID:CreatureID
CreatureFamilies  -->  CreatureDefinition : AdultID:CreatureID
CreatureFamilies  -->  CreatureDefinition : OffspringID:CreatureID
CurriculumDynamic  -->  CurriculumTypes : CurriculumID:CurriculumTypeID
CurriculumDynamic  -->  Seasons : Season:SeasonID
CurriculumEOYRewards  -->  Registry : KnowledgeCard:RegistryID
CurriculumEOYRewards  -->  VirtualContainerList : Reward:VContainerID
CurriculumProfessorDynamic  -->  Registry : ProfessorID:RegistryID
CurriculumRewards  -->  CurriculumTypes : CurriculumID:CurriculumTypeID
CurriculumRewards  -->  Registry : KnowledgeCard:RegistryID
CurriculumRewards  -->  Seasons : Season:SeasonID
CurriculumRewards  -->  VirtualContainerList : Reward:VContainerID
CurriculumTurnInDefinitions  -->  CurriculumTurnInTypes : TurnInType:TypeID
CurriculumTurnInDefinitions  -->  CurriculumTypes : CurriculumID:CurriculumTypeID
CurriculumTurnInDefinitions  -->  CurriculumYear : Year
CurriculumTurnInDefinitions  -->  Registry : TurnInID:RegistryID
CurriculumTurnInDefinitions  -->  Registry : TurnInNPC:RegistryID
CurriculumTurnInDynamic  -->  CurriculumTurnInTypes : TurnInType:TypeValue
CurriculumTurnInDynamic  -->  CurriculumTypes : CurriculumID:CurriculumTypeID
CurriculumTurnInDynamic  -->  CurriculumYear : Year
CurriculumTurnInDynamic  -->  Registry : TurnInID:RegistryID
DuelTechniques  -->  DuelTechniqueCategory : DTCategory:CategoryID
DuelTechniques  -->  DuelTechniqueDifficulty : Difficulty:DuelTechniqueDifficultyID
DuelTechniques  -->  DuelTechniqueRequirementFunction : PerkRequirementFunction:FunctionID
DuelTechniques  -->  DuelTechniqueRequirementFunction : SpellRequirementFunction:FunctionID
DuelTechniques  -->  DuelTechniqueSubtype : Subtype:DuelTechniqueSubtypeID
DuelTechniques  -->  EnvironmentObstacleTypes : EnvironmentObstacleID_2:EnvironmentObstacleTypeID
DuelTechniques  -->  EnvironmentObstacleTypes : EnvironmentObstacleID_1:EnvironmentObstacleTypeID
DuelTechniques  -->  EnvironmentObstacleTypes : EnvironmentObstacleID_3:EnvironmentObstacleTypeID
DuelTechniques  -->  ItemDefinition : ItemID_3:ItemID
DuelTechniques  -->  ItemDefinition : ItemID_1:ItemID
DuelTechniques  -->  ItemDefinition : ItemID_2:ItemID
DuelTechniques  -->  LockDefinition : SpellID_1:LockID
DuelTechniques  -->  LockDefinition : SpellID_2:LockID
DuelTechniques  -->  LockDefinition : SpellID_4:LockID
DuelTechniques  -->  LockDefinition : SpellID_3:LockID
DuelTechniques  -->  PerkDefinition : PerkID_4:PerkID
DuelTechniques  -->  PerkDefinition : PerkID_2:PerkID
DuelTechniques  -->  PerkDefinition : PerkID_3:PerkID
DuelTechniques  -->  PerkDefinition : PerkID_1:PerkID
DuelTechniquesEncounterDynamic  -->  DuelTechniques : DuelTechniqueID
DuelTechniquesEnemyEncounterWeightOverrides  -->  EnemyDefinition : EnemyID
DuelTechniquesEnemyIDRequirement  -->  DuelTechniques : DuelTechniqueID
DuelTechniquesEnemyIDRequirement  -->  EnemyDefinition : EnemyID
DuelTechniquesEnemyPropertyRequirement  -->  DuelTechniques : DuelTechniqueID
DuelTechniquesEnemyPropertyRequirement  -->  DuelTechniquesEnemyProperties : Property1:Property
DuelTechniquesEnemyPropertyRequirement  -->  DuelTechniquesEnemyProperties : Property2:Property
DuelTechniquesLocks  -->  DuelTechniques : DuelTechniqueID
DuelTechniquesLocks  -->  LockDefinition : LockID
DuelTechniques_ComboColumns  -->  DuelTechniqueFirstState : InitialState:DuelTechniqueFirstStateID
DuelTechniques_ComboColumns  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_ComboColumns  -->  SpellKnowledge : FinishingSpellID_2:SpellTypeID
DuelTechniques_ComboColumns  -->  SpellKnowledge : FinishingSpellID_1:SpellTypeID
DuelTechniques_ComboColumns  -->  SpellKnowledge : FinishingSpellID_3:SpellTypeID
DuelTechniques_CountGoalOverrides  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_CustomEventColumns  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_DamageColumns  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_DamageColumns  -->  SpellKnowledge : DamageSpellID_1:SpellTypeID
DuelTechniques_DamageColumns  -->  SpellKnowledge : DamageSpellID_3:SpellTypeID
DuelTechniques_DamageColumns  -->  SpellKnowledge : DamageSpellID_2:SpellTypeID
DuelTechniques_DamageColumns  -->  SpellKnowledge : DamageSpellID_4:SpellTypeID
DuelTechniques_DepulsoColumns  -->  DuelTechniqueFirstState : LaunchActorState:DuelTechniqueFirstStateID
DuelTechniques_DepulsoColumns  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_OppugnoColumns  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_SpellEffectColumns  -->  DuelTechniques : DuelTechniqueID
DuelTechniques_SpellEffectColumns  -->  SpellKnowledge : AffectingSpellID_2:SpellTypeID
DuelTechniques_SpellEffectColumns  -->  SpellKnowledge : AffectingSpellID_3:SpellTypeID
DuelTechniques_SpellEffectColumns  -->  SpellKnowledge : AffectingSpellID_1:SpellTypeID
DuelTechniques_TimedEncounterOverrides  -->  EnemyDefinition : EnemyID
DuelTechniques_TimedJuggleColumns  -->  DuelTechniques : DuelTechniqueID
DungeonEntrances  -->  ItemDefinition : Resource1:ItemID
DungeonEntrances  -->  ItemDefinition : Resource3:ItemID
DungeonEntrances  -->  ItemDefinition : Resource5:ItemID
DungeonEntrances  -->  ItemDefinition : Resource6:ItemID
DungeonEntrances  -->  ItemDefinition : Resource4:ItemID
DungeonEntrances  -->  ItemDefinition : Resource7:ItemID
DungeonEntrances  -->  ItemDefinition : Resource2:ItemID
DungeonEntrances  -->  SpellKnowledge : CompletionSpell1:SpellTypeID
DungeonEntrances  -->  SpellKnowledge : CompletionSpell2:SpellTypeID
DungeonEntrances  -->  SpellKnowledge : CompletionSpell3:SpellTypeID
DungeonEntrances  -->  SpellKnowledge : CompletionSpell5:SpellTypeID
DungeonEntrances  -->  SpellKnowledge : CompletionSpell4:SpellTypeID
EavesdropCharacters  -->  Registry : RegistryID
EavesdropConversations  -->  EavesdropCharacters : Participant1:Abbreviation
EavesdropConversations  -->  EavesdropCharacters : Participant3:Abbreviation
EavesdropConversations  -->  EavesdropCharacters : Participant2:Abbreviation
EavesdropConversations  -->  EavesdropCharacters : Participant4:Abbreviation
EavesdropConversations  -->  EavesdropLocations : Location:Abbreviation
EavesdropLocations  -->  Locations : LocationID
EncounterExclusions  -->  EncounterInstance : EncounterGUID:GUID
EncounterExclusions  -->  EnemyDefinition : EnemyType:EnemyID
EncounterExclusions  -->  Subtypes : SubType:SubtypeID
EncounterInclusions  -->  EncounterInstance : EncounterGUID:GUID
EncounterInclusions  -->  EnemyDefinition : EnemyType:EnemyID
EncounterInclusions  -->  Subtypes : SubType:SubtypeID
EncounterInstance  -->  EncounterScoreModifier : eModifier:EncounterLevel
EncounterInstance  -->  EnemyStatus : eStatusCap:StatusType
EncounterSpawnZones  -->  EnemySize : eSizeCap:Type
EncounterSpawnZones  -->  SpawnLocationTypes : eSpawnType:TypeName
EnemyAggressivenessParams  -->  EnemyAttackExecuteCooldownScale : AttackExecuteCooldownChangeScale:Level
EnemyAttackData  -->  EnemyAttackIDs : AttackID
EnemyAttackData  -->  EnemyAttackScore : AttackScore:Name
EnemyAttackData  -->  EnemyAttackScoreLevel : ScoreLevel:Name
EnemyAttackData  -->  EnemyAttackTicket : AttackTicket2:AttackTicket
EnemyAttackData  -->  EnemyAttackTicket : AttackTicket
EnemyAttackData  -->  EnemyAttackTicket : AttackTicket3:AttackTicket
EnemyAttackData  -->  EnemyDamageLevels : DamageLevel
EnemyAttackData  -->  EnemyDefinition : EnemyID
EnemyAttackData  -->  EnemyParryCounter : ParryCounterType:Type
EnemyAttackData  -->  EnemyParryCounterStyle : ParryCounterStyle:Style
EnemyAttackData  -->  EnemyParryDodge : ParryDodgeStyle:Style
EnemyAttackData  -->  EnemyParryResponse : ParryResponseType:Type
EnemyAttackData  -->  EnemyParryStep : ParryCounterStepDirection:Direction
EnemyAttackData  -->  EnemyShieldBreaker : UnblockableByNPC:Level
EnemyAttackIDs  -->  Registry : AttackID:RegistryID
EnemyAttackModifier  -->  Subtypes : AttackerSubTypeID:SubtypeID
EnemyAttackModifier  -->  Subtypes : TargetSubTypeID:SubtypeID
EnemyAttackParams  -->  EnemyAttackTicket : AttackTicket
EnemyAttackParams  -->  EnemyTicketCooldownScale : TicketCooldownScale:Type
EnemyAttackParams  -->  EnemyTicketLevelDiffScale : TicketLevelDiffScale:Type
EnemyAttackSelectionData  -->  Registry : AttackName:RegistryID
EnemyAttackWeights  -->  EnemyAttackIDs : AttackID
EnemyAttackWeights  -->  Registry : EnemyID:RegistryID
EnemyConfigurationOverrides  -->  Registry : ScalingDataID:RegistryID
EnemyConfigurationOverrides  -->  Registry : CharacterID:RegistryID
EnemyConfigurationOverrides  -->  Registry : AttackDataID:RegistryID
EnemyConfigurationOverrides  -->  Registry : LoadoutID:RegistryID
EnemyConfigurationOverrides  -->  Registry : DefenseDataID:RegistryID
EnemyConfigurationOverrides  -->  Registry : EnemyDefinitionID:RegistryID
EnemyDamageParams  -->  EnemyLevelParams : Level
EnemyDefenseParams  -->  EnemyDefinition : EnemyID
EnemyDefenseParams  -->  EnemyShieldTypes : DefenseLevel:Type
EnemyDefinition  -->  EnemyAccuracyParams : Accuracy:Level
EnemyDefinition  -->  EnemyAggressivenessParams : Aggressiveness:Level
EnemyDefinition  -->  EnemyAgilityParams : Agility:Level
EnemyDefinition  -->  EnemyCombatPositioningParams : CombatPositioning:Level
EnemyDefinition  -->  EnemyDamageParams : Damage:Level
EnemyDefinition  -->  EnemyIdle : Idle:Type
EnemyDefinition  -->  EnemyLevelTicketCooldownScale : TicketCooldown:Type
EnemyDefinition  -->  EnemySize : Size:Type
EnemyDefinition  -->  EnemyStatus : Status:StatusType
EnemyDefinition  -->  ItemDefinition : Drop2:ItemID
EnemyDefinition  -->  ItemDefinition : Drop3:ItemID
EnemyDefinition  -->  ItemDefinition : Drop1:ItemID
EnemyDefinition  -->  KnowledgeActions : KilledKnowledgeAction:EKnowledgeAction
EnemyDefinition  -->  Registry : EnemyID:RegistryID
EnemyDefinitionDuelTechniqueCachedProperties  -->  EnemyDefinition : EnemyID
EnemyDefinitionFallback  -->  LockDefinition : ProgressLockID:LockID
EnemyDefinitionFallback  -->  Registry : RegistryID
EnemyDefinitionFallback  -->  Registry : FallbackID:RegistryID
EnemyDefinitionGroup  -->  EnemyDefinition : ClassID:EnemyID
EnemyDefinitionMap  -->  EnemyDefinition : EnemyClass:EnemyID
EnemyDefinitionMap  -->  Registry : RegistryID
EnemyDefinitionNamed  -->  EnemyDefinition : ObjectClass:EnemyID
EnemyDefinitionNamed  -->  LockDefinition : KilledLockID:LockID
EnemyDefinitionNamed  -->  LootCategories : LootDrop:CategoryID
EnemyDefinitionNamed  -->  Registry : RegistryID
EnemyDefinitionRedirect  -->  EnemyDefinition : ObjectClass:EnemyID
EnemyDefinitionRedirect  -->  Registry : RegistryID
EnemyIdleParams  -->  EnemyLevelParams : Level
EnemyParryData  -->  EnemyAttackIDs : AttackID
EnemyParryData  -->  EnemyDefinition : EnemyID
EnemyPerceptionScores  -->  EnemyPerceptionScoreType : Type
EnemySubtypeData  -->  Subtypes : SubtypeID
EnemyVulnerableDamageMods  -->  EnemyDefinition : EnemyID
EnemyVulnerableDamageMods  -->  EnemyDifficultyScaling : Difficulty:Level
EquippedGearDynamic  -->  GearItems : GearID
EquippedGearDynamic  -->  GearSlotTypes : SlotID
EvilEffectivenessItems  -->  ItemDefinition : ItemID
ExpansionTentNPCs  -->  CharacterDefinition : CharacterID
ExpansionTentNPCs  -->  StatsDynamic : StatID
ExpansionTents  -->  Locations : LocationID
FastTravelLocations  -->  FastTravelRegions : WorldName:RegionID
FertilizerDefinition  -->  ItemDefinition : FertilizerID:ItemID
FilterPopulation  -->  CharacterDefinition : CharacterID
ForcedGearAppearanceDynamic  -->  GearAppearanceItems : GearAppearanceID
ForcedGearAppearanceDynamic  -->  GearSlotTypes : GearSlotType:SlotID
GearAbilityDefinition  -->  IdentityTypes : IdentityType:TypeID
GearItems  -->  GearAppearanceItems : GearAppearanceID
GearItems  -->  GearSlotTypes : SlotID
GearItems  -->  ItemDefinition : GearID:ItemID
GearItemsDynamic  -->  GearItems : GearAppearanceOverrideID:GearID
GearItemsDynamic  -->  GearItems : GearID
GearSlotTypeMapping  -->  GearSlotTypes : SlotID
GearSlotTypeMapping  -->  OutfitItemTypes : OutfitItemType:OutfitItemTypeID
GearSlotTypes  -->  GearItems : DefaultGearID:GearID
GearStatUpgrade  -->  ItemDefinition : ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : Component6:ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : Component5:ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : Component2:ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : Component4:ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : Component3:ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : RecipeItem:ItemID
GearTraitRecipeDefinition  -->  ItemDefinition : Component1:ItemID
GearTraitRecipeDefinition  -->  LockDefinition : LockID
GroupDefinition  -->  GroupTypes : GroupType
GroupMembers  -->  GroupDefinition : GroupID
HoboGeneralTraffic  -->  CharacterDefinition : CharacterID
HogwartsMapIconTable  -->  MapHogwartsLocations : Region:Name
Houses  -->  Locations : DormLocationID:LocationID
InventoryDynamic  -->  ItemDefinition : ItemID
InventoryHolderSlotExpansions  -->  InventoryHolderDefinition : InventoryHolderID
InventoryHolderSlotExpansions  -->  LockDefinition : LockID
ItemDefinition  -->  InventoryHolderDefinition : StorageLocation:InventoryHolderID
ItemDefinition  -->  InventorySlotDefinition : SlotLevel
ItemDefinition  -->  ItemTypes : ItemType:ItemTypes
ItemDefinition  -->  ItemTypes : ItemType2:ItemTypes
ItemDefinition  -->  ItemUsageTypes : ItemUsagetype:ItemUsageType
ItemDefinition  -->  LockDefinition : LockID
ItemDefinition  -->  LockDefinition : PrerequisiteLockID:LockID
ItemDefinition  -->  LockDefinition : PrerequisiteLockID2:LockID
ItemDefinition  -->  LockDefinition : OnUseLockID:LockID
ItemDefinition  -->  RarityTierType : RarityTier:TypeID
ItemDefinition  -->  Registry : ItemID:RegistryID
ItemKnowledgeCardMap  -->  ItemDefinition : ItemID
ItemKnowledgeCardMap  -->  KnowledgeSubjects : KnowledgeCard3:SubjectID
ItemKnowledgeCardMap  -->  KnowledgeSubjects : KnowledgeCard2:SubjectID
ItemKnowledgeCardMap  -->  KnowledgeSubjects : KnowledgeCard1:SubjectID
ItemUseRestrictionDefinition  -->  ItemDefinition : ItemID
ItemUseRestrictionDefinition  -->  ItemUseRestrictionTypes : RestrictionType
ItemUsesAndSources  -->  Registry : ItemID:RegistryID
ItemsDynamic  -->  ItemDefinition : WorldObjectID:ItemID
KnowledgeActions  -->  KnowledgeApplicability : EKnowledgeApplicability
KnowledgeActions  -->  KnowledgeLevels : EKnowledgeLevel
KnowledgeCardPerks  -->  KnowledgeLevels : KnowledgeLevel:EKnowledgeLevel
KnowledgeCardPerks  -->  KnowledgeSubjects : SubjectID
KnowledgeFactTypes  -->  KnowledgeCategories : KnowledgeCategory:KnowledgeCategoryID
KnowledgeFactTypes  -->  UIKnowledgeCategories : UI_Category:CategoryID
KnowledgeFacts  -->  KnowledgeFactTypes : ColumnID
KnowledgeFacts  -->  KnowledgeLevels : EKnowledgeLevel
KnowledgeFacts  -->  KnowledgeSubjects : SubjectID
KnowledgeHogwartsFacts  -->  Locations : LocationID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource7:ItemID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource5:ItemID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource6:ItemID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource3:ItemID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource1:ItemID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource4:ItemID
KnowledgeLocationFacts  -->  ItemDefinition : RegionResource2:ItemID
KnowledgeSubjects  -->  KnowledgeCategories : SubjectCategory:KnowledgeCategoryID
KnowledgeSubjects  -->  LockDefinition : AwardOnUnlock:LockID
KnowledgeVendorFacts  -->  CharacterDefinition : Vendor1:CharacterID
KnowledgeVendorFacts  -->  CharacterDefinition : Vendor2:CharacterID
KnowledgeVendorFacts  -->  CharacterDefinition : Vendor3:CharacterID
LocationNamedVolumes  -->  Locations : LocationID
LockDefinition  -->  LockMessages : LockMsg
LockDefinition  -->  LockTypes : LockTypeID
LockProgression  -->  LockDefinition : LockID
LockProgression  -->  LockDefinition : ActionData:LockID
LockTypes  -->  LockStates : ELockState0:ELockStates
LockTypes  -->  LockStates : ELockState1:ELockStates
LocksDynamic  -->  LockDefinition : LockID
LocksDynamic  -->  LockStates : ELockState:ELockStates
LootCategories  -->  LootCategoryTypes : TypeID:CategoryTypeID
LootCategories  -->  LootRollTypes : RollType:RollTypes
LootContainerContents  -->  KnowledgeLevels : KnowledgeLevel:EKnowledgeLevel
LootContainerContents  -->  LockDefinition : RequiredUnlock:LockID
LootContainerContents  -->  LootCategories : LootCategoryID:CategoryID
LootContainerContents  -->  LootGenerationType : GenerationType
LootContainerContents  -->  Registry : Knowledge:RegistryID
LootContainerContents  -->  VirtualContainerList : ContainerID:VContainerID
LootItemsDynamic  -->  ItemDefinition : ItemID
LootTrackingDynamic  -->  LootCategories : LootCategoryID:CategoryID
LootTrackingDynamic  -->  VirtualContainerList : ContainerID:VContainerID
MapHogwartsLocations  -->  MapHogwartsRegions : Region:Name
MapLocationHints  -->  MapGreaterRegions : GreaterRegion:GreaterRegionName
MissionContainerDynamic  -->  MissionDefinition : MissionID
MissionDefinition  -->  AchievementDefinition : AchievementID
MissionDefinition  -->  LockDefinition : ProgressLockID:LockID
MissionDefinition  -->  LockDefinition : MissionPrereqLockID2:LockID
MissionDefinition  -->  LockDefinition : MissionPrereqLockID1:LockID
MissionDefinition  -->  MissionDefinition : ParentMissionID:MissionID
MissionDefinition  -->  MissionKnowledgeSubjects : KnowledgeSubject
MissionDefinition  -->  MissionLines : MissionLineID
MissionDynamic  -->  MissionDefinition : MissionID
MissionLighthouseSubgoals  -->  MissionDefinition : MissionID
MissionLighthouseSubgoals  -->  MissionLighthouseGoals : LighthouseGoalID
MissionNamedGroups  -->  CharacterDefinition : CharacterID
MissionRewards  -->  MissionDefinition : MissionID
MissionRewards  -->  MissionRewardTypes : TypeID
MissionRewards  -->  MissionRewardUICategories : UICategoryID
MissionSteps  -->  MissionDefinition : MissionID
MissionSteps  -->  MissionTaskTypes : TaskTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword7Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword10Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword9Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword4Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword2Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword11Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword5Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword1Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword8Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword3Type:TaskKeywordTypeID
MissionTaskTypes  -->  MissionTaskKeywordType : Keyword6Type:TaskKeywordTypeID
NPCLevelScaling  -->  NPCMultiplierData : DamageModLevel:Level
NPCLevelScaling  -->  NPCMultiplierData : HealthModLevel:Level
NPCLevelScaling  -->  Registry : CharacterID:RegistryID
NPCSpellLoadouts  -->  Registry : Name:RegistryID
NPCSpellLoadouts  -->  SpellKnowledge : DefaultSpell:SpellTypeID
NPCSpellLoadouts  -->  SpellKnowledge : CombatSpell6:SpellTypeID
NPCSpellLoadouts  -->  SpellKnowledge : CombatSpell5:SpellTypeID
NPCSpellLoadouts  -->  SpellKnowledge : CombatSpell3:SpellTypeID
NPCSpellLoadouts  -->  SpellKnowledge : CombatSpell4:SpellTypeID
NPCSpellLoadouts  -->  SpellKnowledge : CombatSpell1:SpellTypeID
NPCSpellLoadouts  -->  SpellKnowledge : CombatSpell2:SpellTypeID
NamedCreatureDefinition  -->  CreatureColorVariation : ColorVariation
NamedCreatureDefinition  -->  CreatureDefinition : TypeID:CreatureID
NamedCreatureDefinition  -->  Registry : NamedCreatureID:RegistryID
Noise  -->  GameEventIntensity : Intensity:EGameEvent_Intensity
ObjectLocations  -->  Locations : LocationID
ObjectLocations  -->  Registry : ObjectID:RegistryID
PerkDefinition  -->  LockDefinition : LockRequirement2:LockID
PerkDefinition  -->  LockDefinition : LockRequirement:LockID
PerkDefinition  -->  PerkTypes : PerkType:PerkTypeID
PlantDefinition  -->  ItemDefinition : Plant_Product:ItemID
PlantDefinition  -->  LockDefinition : Plant_LockID:LockID
PlantDefinition  -->  PlantSizes : PlotSize:PlantSizeID
PlantDefinition  -->  Registry : PlantID:RegistryID
PlantDefinition  -->  Seasons : SeasonID
PlotDefinition  -->  PlantSizes : PlotSize:PlantSizeID
PlotDefinition  -->  Registry : PlotID:RegistryID
PlotDynamic  -->  ItemDefinition : FertilizedWith:ItemID
PlotDynamic  -->  PlantDefinition : PlantID
PlotDynamic  -->  PlotDefinition : PlotID
PostDeathParams  -->  PostDeathCleanUpEffects : CleanUpEffect
PostDeathParams  -->  PostDeathCleanUpModes : CleanUpMode:CleanUpModes
PostDeathParams  -->  PostDeathSortingModes : SortingMode
PotionDefinition  -->  BrewingUICategories : UICategory:Category
PotionDefinition  -->  ItemDefinition : Ingredient6:ItemID
PotionDefinition  -->  ItemDefinition : Ingredient4:ItemID
PotionDefinition  -->  ItemDefinition : Ingredient3:ItemID
PotionDefinition  -->  ItemDefinition : Ingredient5:ItemID
PotionDefinition  -->  ItemDefinition : Ingredient1:ItemID
PotionDefinition  -->  ItemDefinition : Ingredient2:ItemID
PotionDefinition  -->  LockDefinition : LockID
PotionDefinition  -->  PotionTypes : PotionTypeID
PotionDefinition  -->  Registry : PotionID:RegistryID
RPGAbilityDurationDefinition  -->  PotionUnitTypes : Units:UnitID
RPGAbilityDurationDefinition  -->  Registry : AbilityID:RegistryID
RPGPermaAbilityDynamic  -->  Registry : ActorID:RegistryID
RPGSystemCooldowns  -->  ItemDefinition : AbilityName:ItemID
RPGSystemCooldowns  -->  RPGSystemCooldownDefinition : CooldownGroup:CooldownName
Registry  -->  Subtypes : SubtypeID
RichPaperDefinition  -->  RichPaperTypes : RichPaperTypeID
SanctuaryAreas  -->  ConjurationContext : ConjurationContext
SanctuaryBiomeDefinition  -->  NurturingSpaceDefinition : NurturingSpaceID
SanctuaryBiomeDefinition  -->  SanctuaryAreas : BiomeID:AreaID
SanctuaryBiomeDynamic  -->  SanctuaryBiomeDefinition : BiomeID
SanctuaryExpansionDefinition  -->  LockDefinition : ExpansionLockID:LockID
SanctuaryExpansionDefinition  -->  SanctuaryAreas : AreaID
SanctuaryHousekeepingDynamic  -->  SanctuaryHousekeepingDefinition : Type
SanctuaryInitialCustomizationChoices  -->  LockDefinition : DressingLock:LockID
SanctuaryInitialCustomizationChoices  -->  TransfigurationColors : StructureColor:Color
SanctuaryItemGeneratorData  -->  LootCategories : LootCategoryID:CategoryID
SanctuaryItemGeneratorData  -->  TransfigurationObjects : ItemGenerator:Category
ScheduleDynamic  -->  Registry : CharacterID:RegistryID
Schedule_Azkaban  -->  ActivityDefinition : ActivityID
Schedule_Azkaban  -->  Locations : OverrideLocationID:LocationID
Schedule_Azkaban  -->  Registry : CharacterID:RegistryID
Schedule_Azkaban  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Azkaban  -->  StationPropTypes : PropTypeID
Schedule_Cairn_Dungeon_2  -->  ActivityDefinition : ActivityID
Schedule_Cairn_Dungeon_2  -->  Locations : OverrideLocationID:LocationID
Schedule_Cairn_Dungeon_2  -->  Registry : CharacterID:RegistryID
Schedule_Cairn_Dungeon_2  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cairn_Dungeon_2  -->  StationPropTypes : PropTypeID
Schedule_Cairn_Dungeon_20  -->  ActivityDefinition : ActivityID
Schedule_Cairn_Dungeon_20  -->  Locations : OverrideLocationID:LocationID
Schedule_Cairn_Dungeon_20  -->  Registry : CharacterID:RegistryID
Schedule_Cairn_Dungeon_20  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cairn_Dungeon_20  -->  StationPropTypes : PropTypeID
Schedule_Cairn_Dungeon_21  -->  ActivityDefinition : ActivityID
Schedule_Cairn_Dungeon_21  -->  Locations : OverrideLocationID:LocationID
Schedule_Cairn_Dungeon_21  -->  Registry : CharacterID:RegistryID
Schedule_Cairn_Dungeon_21  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cairn_Dungeon_21  -->  StationPropTypes : PropTypeID
Schedule_Cairn_Dungeon_3  -->  ActivityDefinition : ActivityID
Schedule_Cairn_Dungeon_3  -->  Locations : OverrideLocationID:LocationID
Schedule_Cairn_Dungeon_3  -->  Registry : CharacterID:RegistryID
Schedule_Cairn_Dungeon_3  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cairn_Dungeon_3  -->  StationPropTypes : PropTypeID
Schedule_Cairn_Dungeon_8  -->  ActivityDefinition : ActivityID
Schedule_Cairn_Dungeon_8  -->  Locations : OverrideLocationID:LocationID
Schedule_Cairn_Dungeon_8  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cairn_Dungeon_8  -->  StationPropTypes : PropTypeID
Schedule_Castle_Dungeon_1  -->  ActivityDefinition : ActivityID
Schedule_Castle_Dungeon_1  -->  Locations : OverrideLocationID:LocationID
Schedule_Castle_Dungeon_1  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Castle_Dungeon_1  -->  StationPropTypes : PropTypeID
Schedule_Castle_Dungeon_10  -->  ActivityDefinition : ActivityID
Schedule_Castle_Dungeon_10  -->  Locations : OverrideLocationID:LocationID
Schedule_Castle_Dungeon_10  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Castle_Dungeon_10  -->  StationPropTypes : PropTypeID
Schedule_Castle_Dungeon_11  -->  ActivityDefinition : ActivityID
Schedule_Castle_Dungeon_11  -->  Locations : OverrideLocationID:LocationID
Schedule_Castle_Dungeon_11  -->  Registry : CharacterID:RegistryID
Schedule_Castle_Dungeon_11  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Castle_Dungeon_11  -->  StationPropTypes : PropTypeID
Schedule_Castle_Dungeon_15  -->  ActivityDefinition : ActivityID
Schedule_Castle_Dungeon_15  -->  Locations : OverrideLocationID:LocationID
Schedule_Castle_Dungeon_15  -->  Registry : CharacterID:RegistryID
Schedule_Castle_Dungeon_15  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Castle_Dungeon_15  -->  StationPropTypes : PropTypeID
Schedule_Castle_Dungeon_19  -->  ActivityDefinition : ActivityID
Schedule_Castle_Dungeon_19  -->  Locations : OverrideLocationID:LocationID
Schedule_Castle_Dungeon_19  -->  Registry : CharacterID:RegistryID
Schedule_Castle_Dungeon_19  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Castle_Dungeon_19  -->  StationPropTypes : PropTypeID
Schedule_Castle_Dungeon_22  -->  ActivityDefinition : ActivityID
Schedule_Castle_Dungeon_22  -->  Locations : OverrideLocationID:LocationID
Schedule_Castle_Dungeon_22  -->  Registry : CharacterID:RegistryID
Schedule_Castle_Dungeon_22  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Castle_Dungeon_22  -->  StationPropTypes : PropTypeID
Schedule_Cav_Dungeon_01  -->  ActivityDefinition : ActivityID
Schedule_Cav_Dungeon_01  -->  Locations : OverrideLocationID:LocationID
Schedule_Cav_Dungeon_01  -->  Registry : CharacterID:RegistryID
Schedule_Cav_Dungeon_01  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cav_Dungeon_01  -->  StationPropTypes : PropTypeID
Schedule_Cav_Dungeon_02  -->  ActivityDefinition : ActivityID
Schedule_Cav_Dungeon_02  -->  Locations : OverrideLocationID:LocationID
Schedule_Cav_Dungeon_02  -->  Registry : CharacterID:RegistryID
Schedule_Cav_Dungeon_02  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cav_Dungeon_02  -->  StationPropTypes : PropTypeID
Schedule_Cav_Dungeon_05  -->  ActivityDefinition : ActivityID
Schedule_Cav_Dungeon_05  -->  Locations : OverrideLocationID:LocationID
Schedule_Cav_Dungeon_05  -->  Registry : CharacterID:RegistryID
Schedule_Cav_Dungeon_05  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cav_Dungeon_05  -->  StationPropTypes : PropTypeID
Schedule_Cav_Dungeon_08  -->  ActivityDefinition : ActivityID
Schedule_Cav_Dungeon_08  -->  Locations : OverrideLocationID:LocationID
Schedule_Cav_Dungeon_08  -->  Registry : CharacterID:RegistryID
Schedule_Cav_Dungeon_08  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cav_Dungeon_08  -->  StationPropTypes : PropTypeID
Schedule_Cav_Dungeon_12  -->  ActivityDefinition : ActivityID
Schedule_Cav_Dungeon_12  -->  Locations : OverrideLocationID:LocationID
Schedule_Cav_Dungeon_12  -->  Registry : CharacterID:RegistryID
Schedule_Cav_Dungeon_12  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cav_Dungeon_12  -->  StationPropTypes : PropTypeID
Schedule_Cavern_Dungeon_10  -->  ActivityDefinition : ActivityID
Schedule_Cavern_Dungeon_10  -->  Locations : OverrideLocationID:LocationID
Schedule_Cavern_Dungeon_10  -->  Registry : CharacterID:RegistryID
Schedule_Cavern_Dungeon_10  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cavern_Dungeon_10  -->  StationPropTypes : PropTypeID
Schedule_Cavern_Dungeon_19  -->  ActivityDefinition : ActivityID
Schedule_Cavern_Dungeon_19  -->  Locations : OverrideLocationID:LocationID
Schedule_Cavern_Dungeon_19  -->  Registry : CharacterID:RegistryID
Schedule_Cavern_Dungeon_19  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cavern_Dungeon_19  -->  StationPropTypes : PropTypeID
Schedule_Cavern_Dungeon_24  -->  ActivityDefinition : ActivityID
Schedule_Cavern_Dungeon_24  -->  Locations : OverrideLocationID:LocationID
Schedule_Cavern_Dungeon_24  -->  Registry : CharacterID:RegistryID
Schedule_Cavern_Dungeon_24  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cavern_Dungeon_24  -->  StationPropTypes : PropTypeID
Schedule_Cavern_Dungeon_26  -->  ActivityDefinition : ActivityID
Schedule_Cavern_Dungeon_26  -->  Locations : OverrideLocationID:LocationID
Schedule_Cavern_Dungeon_26  -->  Registry : CharacterID:RegistryID
Schedule_Cavern_Dungeon_26  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cavern_Dungeon_26  -->  StationPropTypes : PropTypeID
Schedule_Cavern_Dungeon_33  -->  ActivityDefinition : ActivityID
Schedule_Cavern_Dungeon_33  -->  Locations : OverrideLocationID:LocationID
Schedule_Cavern_Dungeon_33  -->  Registry : CharacterID:RegistryID
Schedule_Cavern_Dungeon_33  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cavern_Dungeon_33  -->  StationPropTypes : PropTypeID
Schedule_Cavern_Dungeon_34  -->  ActivityDefinition : ActivityID
Schedule_Cavern_Dungeon_34  -->  Locations : OverrideLocationID:LocationID
Schedule_Cavern_Dungeon_34  -->  Registry : CharacterID:RegistryID
Schedule_Cavern_Dungeon_34  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Cavern_Dungeon_34  -->  StationPropTypes : PropTypeID
Schedule_DeathHallows_Dungeon  -->  ActivityDefinition : ActivityID
Schedule_DeathHallows_Dungeon  -->  Locations : OverrideLocationID:LocationID
Schedule_DeathHallows_Dungeon  -->  Registry : CharacterID:RegistryID
Schedule_DeathHallows_Dungeon  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_DeathHallows_Dungeon  -->  StationPropTypes : PropTypeID
Schedule_Default  -->  ActivityDefinition : ActivityID
Schedule_Default  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Default  -->  StationPropTypes : PropTypeID
Schedule_Empty  -->  ActivityDefinition : ActivityID
Schedule_Empty  -->  Locations : OverrideLocationID:LocationID
Schedule_Empty  -->  Registry : CharacterID:RegistryID
Schedule_Empty  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Empty  -->  StationPropTypes : PropTypeID
Schedule_GeneratedDefaults  -->  ActivityDefinition : ActivityID
Schedule_GeneratedDefaults  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_GeneratedDefaults  -->  Schedule_GeneratedLocationIds : OverrideLocationID:LocationID
Schedule_GeneratedDefaults  -->  StationPropTypes : PropTypeID
Schedule_GeneratedLocations  -->  ActivityDefinition : ActivityID
Schedule_GeneratedLocations  -->  Locations : OverrideLocationID:LocationID
Schedule_GeneratedLocations  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_GeneratedLocations  -->  StationPropTypes : PropTypeID
Schedule_GobMine_Dungeon_07  -->  ActivityDefinition : ActivityID
Schedule_GobMine_Dungeon_07  -->  Locations : OverrideLocationID:LocationID
Schedule_GobMine_Dungeon_07  -->  Registry : CharacterID:RegistryID
Schedule_GobMine_Dungeon_07  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_GobMine_Dungeon_07  -->  StationPropTypes : PropTypeID
Schedule_GobMine_Dungeon_13  -->  ActivityDefinition : ActivityID
Schedule_GobMine_Dungeon_13  -->  Locations : OverrideLocationID:LocationID
Schedule_GobMine_Dungeon_13  -->  Registry : CharacterID:RegistryID
Schedule_GobMine_Dungeon_13  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_GobMine_Dungeon_13  -->  StationPropTypes : PropTypeID
Schedule_Gobmine_Dungeon_01  -->  ActivityDefinition : ActivityID
Schedule_Gobmine_Dungeon_01  -->  Locations : OverrideLocationID:LocationID
Schedule_Gobmine_Dungeon_01  -->  Registry : CharacterID:RegistryID
Schedule_Gobmine_Dungeon_01  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Gobmine_Dungeon_01  -->  StationPropTypes : PropTypeID
Schedule_Gobmine_Dungeon_06  -->  ActivityDefinition : ActivityID
Schedule_Gobmine_Dungeon_06  -->  Locations : OverrideLocationID:LocationID
Schedule_Gobmine_Dungeon_06  -->  Registry : CharacterID:RegistryID
Schedule_Gobmine_Dungeon_06  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Gobmine_Dungeon_06  -->  StationPropTypes : PropTypeID
Schedule_Gobmine_Dungeon_11  -->  ActivityDefinition : ActivityID
Schedule_Gobmine_Dungeon_11  -->  Locations : OverrideLocationID:LocationID
Schedule_Gobmine_Dungeon_11  -->  Registry : CharacterID:RegistryID
Schedule_Gobmine_Dungeon_11  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Gobmine_Dungeon_11  -->  StationPropTypes : PropTypeID
Schedule_Gobmine_Dungeon_12  -->  ActivityDefinition : ActivityID
Schedule_Gobmine_Dungeon_12  -->  Locations : OverrideLocationID:LocationID
Schedule_Gobmine_Dungeon_12  -->  Registry : CharacterID:RegistryID
Schedule_Gobmine_Dungeon_12  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Gobmine_Dungeon_12  -->  StationPropTypes : PropTypeID
Schedule_HM_ExtortionistHideout  -->  ActivityDefinition : ActivityID
Schedule_HM_ExtortionistHideout  -->  Locations : OverrideLocationID:LocationID
Schedule_HM_ExtortionistHideout  -->  Registry : CharacterID:RegistryID
Schedule_HM_ExtortionistHideout  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_HM_ExtortionistHideout  -->  StationPropTypes : PropTypeID
Schedule_HOG_Dungeon_01  -->  ActivityDefinition : ActivityID
Schedule_HOG_Dungeon_01  -->  Locations : OverrideLocationID:LocationID
Schedule_HOG_Dungeon_01  -->  Registry : CharacterID:RegistryID
Schedule_HOG_Dungeon_01  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_HOG_Dungeon_01  -->  StationPropTypes : PropTypeID
Schedule_HauntedShop_Dungeon_02  -->  ActivityDefinition : ActivityID
Schedule_HauntedShop_Dungeon_02  -->  Locations : OverrideLocationID:LocationID
Schedule_HauntedShop_Dungeon_02  -->  Registry : CharacterID:RegistryID
Schedule_HauntedShop_Dungeon_02  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_HauntedShop_Dungeon_02  -->  StationPropTypes : PropTypeID
Schedule_HauntedShop_Dungeon_03  -->  ActivityDefinition : ActivityID
Schedule_HauntedShop_Dungeon_03  -->  Locations : OverrideLocationID:LocationID
Schedule_HauntedShop_Dungeon_03  -->  Registry : CharacterID:RegistryID
Schedule_HauntedShop_Dungeon_03  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_HauntedShop_Dungeon_03  -->  StationPropTypes : PropTypeID
Schedule_Hogsmeade_Dungeon_02  -->  ActivityDefinition : ActivityID
Schedule_Hogsmeade_Dungeon_02  -->  Locations : OverrideLocationID:LocationID
Schedule_Hogsmeade_Dungeon_02  -->  Registry : CharacterID:RegistryID
Schedule_Hogsmeade_Dungeon_02  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Hogsmeade_Dungeon_02  -->  StationPropTypes : PropTypeID
Schedule_Hogwarts_Dungeon_02  -->  ActivityDefinition : ActivityID
Schedule_Hogwarts_Dungeon_02  -->  Locations : OverrideLocationID:LocationID
Schedule_Hogwarts_Dungeon_02  -->  Registry : CharacterID:RegistryID
Schedule_Hogwarts_Dungeon_02  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Hogwarts_Dungeon_02  -->  StationPropTypes : PropTypeID
Schedule_Hogwarts_Dungeon_Evil  -->  ActivityDefinition : ActivityID
Schedule_Hogwarts_Dungeon_Evil  -->  Locations : OverrideLocationID:LocationID
Schedule_Hogwarts_Dungeon_Evil  -->  Registry : CharacterID:RegistryID
Schedule_Hogwarts_Dungeon_Evil  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Hogwarts_Dungeon_Evil  -->  StationPropTypes : PropTypeID
Schedule_Intro  -->  ActivityDefinition : ActivityID
Schedule_Intro  -->  Locations : OverrideLocationID:LocationID
Schedule_Intro  -->  Registry : CharacterID:RegistryID
Schedule_Intro  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Intro  -->  StationPropTypes : PropTypeID
Schedule_Marketing  -->  ActivityDefinition : ActivityID
Schedule_Marketing  -->  Locations : OverrideLocationID:LocationID
Schedule_Marketing  -->  Registry : CharacterID:RegistryID
Schedule_Marketing  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Marketing  -->  StationPropTypes : PropTypeID
Schedule_Overland  -->  ActivityDefinition : ActivityID
Schedule_Overland  -->  Locations : OverrideLocationID:LocationID
Schedule_Overland  -->  Registry : CharacterID:RegistryID
Schedule_Overland  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Overland  -->  StationPropTypes : PropTypeID
Schedule_Pensieve_Tomb_2  -->  ActivityDefinition : ActivityID
Schedule_Pensieve_Tomb_2  -->  Locations : OverrideLocationID:LocationID
Schedule_Pensieve_Tomb_2  -->  Registry : CharacterID:RegistryID
Schedule_Pensieve_Tomb_2  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Pensieve_Tomb_2  -->  StationPropTypes : PropTypeID
Schedule_PoacherHideout  -->  ActivityDefinition : ActivityID
Schedule_PoacherHideout  -->  Locations : OverrideLocationID:LocationID
Schedule_PoacherHideout  -->  Registry : CharacterID:RegistryID
Schedule_PoacherHideout  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_PoacherHideout  -->  StationPropTypes : PropTypeID
Schedule_RootLevel  -->  ActivityDefinition : ActivityID
Schedule_RootLevel  -->  Locations : OverrideLocationID:LocationID
Schedule_RootLevel  -->  Registry : CharacterID:RegistryID
Schedule_RootLevel  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_RootLevel  -->  StationPropTypes : PropTypeID
Schedule_SancStudy  -->  ActivityDefinition : ActivityID
Schedule_SancStudy  -->  Locations : OverrideLocationID:LocationID
Schedule_SancStudy  -->  Registry : CharacterID:RegistryID
Schedule_SancStudy  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_SancStudy  -->  StationPropTypes : PropTypeID
Schedule_Sanctum_Dungeon_Cavern2  -->  ActivityDefinition : ActivityID
Schedule_Sanctum_Dungeon_Cavern2  -->  Locations : OverrideLocationID:LocationID
Schedule_Sanctum_Dungeon_Cavern2  -->  Registry : CharacterID:RegistryID
Schedule_Sanctum_Dungeon_Cavern2  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_Sanctum_Dungeon_Cavern2  -->  StationPropTypes : PropTypeID
Schedule_SpawnOnly  -->  ActivityDefinition : ActivityID
Schedule_SpawnOnly  -->  Locations : OverrideLocationID:LocationID
Schedule_SpawnOnly  -->  Registry : CharacterID:RegistryID
Schedule_SpawnOnly  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_SpawnOnly  -->  StationPropTypes : PropTypeID
Schedule_ThievesHideout  -->  ActivityDefinition : ActivityID
Schedule_ThievesHideout  -->  Locations : OverrideLocationID:LocationID
Schedule_ThievesHideout  -->  Registry : CharacterID:RegistryID
Schedule_ThievesHideout  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_ThievesHideout  -->  StationPropTypes : PropTypeID
Schedule_ZZS_TrollFight  -->  ActivityDefinition : ActivityID
Schedule_ZZS_TrollFight  -->  ScheduleEntryTypes : EntryTypeID:TypeID
Schedule_ZZS_TrollFight  -->  Schedule_GeneratedLocationIds : OverrideLocationID:LocationID
Schedule_ZZS_TrollFight  -->  StationPropTypes : PropTypeID
SeatFillerSchedule  -->  ActivityTypes : ActivityTypeID
SeatFillerSchedule  -->  Genders : GenderID
SeatFillerSchedule  -->  Houses : HouseID
SeatFillerSchedule  -->  Locations : LocationID
SeatFillerSchedule  -->  Subtypes : SubtypeID
SecretFactsDefinition  -->  KnowledgeSubjects : SubjectID
SocialActionDefinition  -->  SocialActionType : SocialActionTypeID
SocialActionDefinition  -->  SocialCapitalStatuses : MinPropagationSCStatus:SocialCapitalStatusID
SocialActionDynamic  -->  Locations : LocationID
SocialActionDynamic  -->  Registry : TargetCharacterID:RegistryID
SocialActionDynamic  -->  SocialActionDefinition : SocialActionID
SocialActionSemantics  -->  SocialActionDefinition : SocialActionID
SocialActionSemantics  -->  SocialSemantics : SocialSemanticID
SocialInteractionData  -->  CharacterDefinition : CharacterID
SocialInteractionData  -->  LockDefinition : RequiredLock:LockID
SocialInteractionData  -->  MissionDefinition : RequiredMission:MissionID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Stranger:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Indifferent:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Hate:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Companion:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : IsCompanion:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Dislike:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Cordial:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Friendly:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionDisplayStatuses : Familiar:SocialInteractionDisplayStatusID
SocialInteractionData  -->  SocialInteractionTypes : InteractionType:SocialInteractionTypeID
SocialInteractionData  -->  Subtypes : CharacterType:SubtypeID
SocialSemantics  -->  SocialSemanticTypes : SocialSemanticTypeID
SocialStationActionChoices  -->  ActivityTypes : ActivityTypeID
SocialStationActionChoices  -->  SocialActionDefinition : CurrentAction:SocialActionID
SocialStationActionChoices  -->  SocialActionDefinition : AvailableAction:SocialActionID
SocialStationActionChoices  -->  StationPropTypes : PropType:PropTypeID
SpawnGroupDefinition  -->  LockDefinition : RequiredProgressLockID:LockID
SpawnGroupDefinition  -->  Registry : RegistryID
SpawnGroupDefinition  -->  Registry : SpawnID:RegistryID
SpawnGroupDefinition  -->  SpawnLocationTypes : SpawnDiscoveryType:TypeName
SpawnGroupEconomy  -->  Registry : SpawnID:RegistryID
SpawnRestrictionTypes  -->  SpawnRestrictionCategories : RestrictionCategory:CategoryName
SpawnRestrictions  -->  SpawnRestrictionTypes : Type:RestrictionName
SpellDefinition  -->  EnemyShieldBreaker : EnemyShieldBreaker:Level
SpellDefinition  -->  Noise : ImpactNoise:Noise
SpellDefinition  -->  Noise : CastNoise:Noise
SpellDefinition  -->  SpellImpactTypes : ImpactType:EImpactTypesName
SpellDefinition  -->  SpellKnowledge : SpellTypeID
SpellDefinition  -->  SpellSizes : SizeLimit:EObjectSizeClassName
SpellDefinition  -->  SpellUpgrades : Upgrade:SpellUpgrade
SpellKnowledge  -->  KnowledgeActions : KnowledgeGain:EKnowledgeAction
SpellKnowledge  -->  LockDefinition : Lock:LockID
SpellKnowledge  -->  Registry : SpellTypeID:RegistryID
SpellKnowledge  -->  SocialSemantics : CurriculumAssociation:SocialSemanticID
SpellKnowledge  -->  SocialSemantics : SpellIdentity:SocialSemanticID
SpellKnowledge  -->  SpellCategories : SpellCategory:TypeID
SpellKnowledge  -->  SpellUpgrades : UpgradeID0:SpellUpgrade
SpellMappingForLoadouts  -->  SocialSemantics : SocialSemantic:SocialSemanticID
SpellMappingForLoadouts  -->  SpellKnowledge : SpellID:SpellTypeID
SphinxPuzzleDefinition  -->  Registry : SphinxPuzzleID:RegistryID
SphinxPuzzleInstance  -->  SphinxPuzzleDefinition : SphinxPuzzleTypeID:SphinxPuzzleID
StationPropTypes  -->  StationPropClasses : PropClassID
StationSiteVicinityScale  -->  Locations : LocationID
SubjectDefinition  -->  Registry : Professor:RegistryID
SubjectDefinition  -->  SubjectTypes : SubjectTypeID
SubjectOfTheDayKnowledgeCards  -->  KnowledgeSubjects : KnowledgeCard:SubjectID
SubjectOfTheDayKnowledgeCards  -->  LockDefinition : LockID
SubjectOfTheDayKnowledgeCards  -->  SubjectDefinition : SubjectID
SubtypeInteraction  -->  EnemyInteractionTypes : InteractionAfraid:Interaction
SubtypeInteraction  -->  EnemyInteractionTypes : Interaction
SubtypeInteraction  -->  Subtypes : InteractorSubtype:SubtypeID
SubtypeInteraction  -->  Subtypes : InteracteeSubtype:SubtypeID
Subtypes  -->  RegistryTypes : RegistryTypeID
TabooItemList  -->  ItemDefinition : ItemID
TerrainAnchorSpawnGroups  -->  TerrainAnchorGroups : Group2Name:GroupName
TerrainAnchorSpawnGroups  -->  TerrainAnchorGroups : Group1Name:GroupName
TerrainAnchorSpawnGroups  -->  TerrainAnchorGroups : Group4Name:GroupName
TerrainAnchorSpawnGroups  -->  TerrainAnchorGroups : Group3Name:GroupName
TerrainAnchors  -->  TerrainAnchorSpawnGroups : SpawnGroup
TileForegeableSpawning  -->  ForegeableCategoryDefinition : Category
TileForegeableSpawning  -->  Registry : SpawnID:RegistryID
TransfigurationClasses  -->  TransfigurationSlotPools : TransfigSlotTypeID:TransfigSlotID
TransfigurationClasses  -->  TransformationStreamingPriority : StreamingPriority:Priority
TransfigurationClasses  -->  TransformationStyles : TransformationStyle:Style
TransfigurationClasses  -->  VanishmentStyles : VanishmentStyle:Style
TransfigurationDynamic  -->  Registry : TypeID:RegistryID
TransfigurationDynamic  -->  Registry : OriginalTypeID:RegistryID
TransfigurationObjectGroups  -->  TransfigurationGroups : Groupname
TransfigurationObjectGroups  -->  TransfigurationObjects : Category
TransfigurationObjectLocks  -->  LockDefinition : LockID
TransfigurationObjectLocks  -->  Registry : ObjectID:RegistryID
TransfigurationObjectStatsCategories  -->  TransfigurationObjects : ObjectCategory:Category
TransfigurationObjects  -->  ConjurationCategory : ConjurationCategory2:ConjurationCategory
TransfigurationObjects  -->  ConjurationCategory : ConjurationCategory
TransfigurationObjects  -->  ItemDefinition : Resource5_ID:ItemID
TransfigurationObjects  -->  ItemDefinition : Resource1_ID:ItemID
TransfigurationObjects  -->  ItemDefinition : Resource4_ID:ItemID
TransfigurationObjects  -->  ItemDefinition : Resource3_ID:ItemID
TransfigurationObjects  -->  ItemDefinition : Resource2_ID:ItemID
TransfigurationObjects  -->  Registry : Item3:RegistryID
TransfigurationObjects  -->  Registry : Item6:RegistryID
TransfigurationObjects  -->  Registry : Item4:RegistryID
TransfigurationObjects  -->  Registry : Item5:RegistryID
TransfigurationObjects  -->  Registry : Item1:RegistryID
TransfigurationObjects  -->  Registry : Item7:RegistryID
TransfigurationObjects  -->  Registry : Item2:RegistryID
TransfigurationObjects  -->  Registry : Item8:RegistryID
TransfigurationObjects  -->  TransfigurationClasses : Class
TransfigurationObjects  -->  TransfigurationSnapping : Snapping
TransfigurationObjects  -->  TransfigurationSocketCategories : SocketCategory:Category
TransfigurationObjects  -->  TransformationGroups : TransformationGroup:GroupID
TransfigurationSlotPoolExpansions  -->  LockDefinition : LockID
TransfigurationSlotPoolExpansions  -->  TransfigurationSlotPools : SlotID:TransfigSlotID
TransformationOverlandResults  -->  Registry : Transformation2:RegistryID
TransformationOverlandResults  -->  Registry : Transformation4:RegistryID
TransformationOverlandResults  -->  Registry : Transformation3:RegistryID
TransformationOverlandResults  -->  Registry : Transformation1:RegistryID
TransformationOverlandTargets  -->  TransformationOverlandResults : ResultCategory1:ResultCategory
TransformationOverlandTargets  -->  TransformationOverlandResults : ResultCategory2:ResultCategory
TransformationOverlandTargets  -->  TransformationOverlandResults : ResultCategory3:ResultCategory
TransformationOverlandTargets  -->  TransformationOverlandResults : ResultCategory4:ResultCategory
TriggeredEffects  -->  BuffAttributeType : EffectID:AttributeID
TriggeredEffects  -->  Registry : EffectSourceID:RegistryID
TriggeredEffects  -->  TriggeredEffectTypes : EffectType
UIActionGroupDynamic  -->  ItemDefinition : InventoryItem_North:ItemID
UIActionGroupDynamic  -->  ItemDefinition : InventoryItem_South:ItemID
UIActionGroupDynamic  -->  ItemDefinition : InventoryItem_West:ItemID
UIActionGroupDynamic  -->  ItemDefinition : InventoryItem_East:ItemID
UIActionGroupDynamic  -->  SpellKnowledge : Spell_West:SpellTypeID
UIActionGroupDynamic  -->  SpellKnowledge : Spell_South:SpellTypeID
UIActionGroupDynamic  -->  SpellKnowledge : Spell_North:SpellTypeID
UIActionGroupDynamic  -->  SpellKnowledge : Spell_East:SpellTypeID
UIActionItem  -->  ItemDefinition : InventoryItemID:ItemID
UIActionItem  -->  SpellKnowledge : SpellID:SpellTypeID
UIActionItem  -->  WorldObjectDefinition : StorageLocation:WorldObjectID
UIKeyBindingsDynamic  -->  UIInputActions : PS5:ActionID
UIKeyBindingsDynamic  -->  UIInputActions : XboxOne:ActionID
UIKeyBindingsDynamic  -->  UIInputActions : XSX:ActionID
UIKeyBindingsDynamic  -->  UIInputActions : Switch:ActionID
UIKeyBindingsDynamic  -->  UIInputActions : PS4:ActionID
UIKeyBindingsDynamic  -->  UIInputActions : PCKeyboard:ActionID
UIKeyBindingsDynamic  -->  UIInputActions : PCController:ActionID
UIQuickActionsDynamic  -->  ItemDefinition : InventoryItemID:ItemID
UIQuickActionsDynamic  -->  SpellKnowledge : SpellID:SpellTypeID
UIQuickActionsDynamic  -->  WorldObjectDefinition : StorageLocation:WorldObjectID
UITwitchActions  -->  ItemDefinition : ItemID
UITwitchActions  -->  SpellKnowledge : Spell:SpellTypeID
UIWorldActions  -->  UIActionGroupDynamic : FaceButtonActionGroup:GroupID
UIWorldActions  -->  UIActionGroupDynamic : DPadGroup2:GroupID
UIWorldActions  -->  UIActionGroupDynamic : DPadGroup3:GroupID
UIWorldActions  -->  UIActionGroupDynamic : DPadGroup1:GroupID
UIWorldActions  -->  UIActionGroupDynamic : DPadGroup4:GroupID
UIWorldActions  -->  UIActionModes : DefaultActionMode:ModeID
UIWorldActions  -->  WorldObjectDefinition : StorageLocation:WorldObjectID
UnresolvedDoorStatesDynamic  -->  DoorStates : State
VendorStocks  -->  LockDefinition : LockID
VendorStocks  -->  LootCategories : ContainerID:CategoryID
VendorStocks  -->  Registry : VendorID:RegistryID
VendorStocksDynamic  -->  Registry : VendorID:RegistryID
VendorStocksDynamic  -->  VirtualContainerList : ContainerID:VContainerID
VendorUnavailableStock  -->  LockDefinition : Lock:LockID
VendorUnavailableStock  -->  Registry : VendorID:RegistryID
VirtualContainerContents  -->  ItemDefinition : ItemID
VirtualContainerContents  -->  LockDefinition : LockID
VirtualContainerContents  -->  VirtualContainerList : ContainerID:VContainerID
VirtualContainerContents  -->  VirtualContainerList : VContainerID
VirtualContainerList  -->  VirtualContainerTypes : SubtypeID:TypeID
WorldObjectDefinition  -->  Registry : WorldObjectID:RegistryID
WorldObjectDynamic  -->  WorldObjectDefinition : WorldObjectID
WorldRegionAdjustments  -->  WorldAdjustments : Adjustment:Name
WorldRegionAdjustments  -->  WorldRegions : Region:Name
