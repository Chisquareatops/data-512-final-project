# Final Project Proposal

## Data
### Summary
I propose to use the National Health and Aging Trends Study (NHATS) dataset; specifically the final release of rounds one through eight. This dataset contains information from a nationally representative sample of Medicare beneficiaries aged 65 or older. The first sample was interviewed in 2011 and there have been annual follow up interviews, with a replenishment of participants in 2015. An incredible amount of information is gathered from these individuals and other individuals in their social networks, but in particular I am interested in examining the relationship between various disabilities/impairments and social connectedness/participation in valued activities. The data contained in NHATS is not just survey data, but also includes data gathered from performance based tests of physical and cognitive capacity (about which perceptual, self-rated information is also gathered).

### Files
The primary files I will be using are:

NHATS_Round_8_SP_File.dta contains the sample person (SP) and the facility questionnaire (FQ) data (5,547 observations and 1,317 variables). 

NHATS_Round_8_OP_File.dta contains the other person (OP) data (46,905 observations and 571 
variables). 

NHATS_Round_8_Tracker_File.dta contains tracking information for all persons sampled for NHATS (19,530 observations and 889 variables).

This data is publically available from https://www.nhats.org. Registration is required to access the data files.

## Project Description
### Hypothesis
My primary hypothesis is that increasing levels of disability, particularly cognitive impairment, will correlate with decreasing levels of participation in valued activities and a narrowing of the social circle. A secondary hypothesis is that this association will be less pronounced in individuals who are able to age in place (i.e. remain in their homes).

### Variables
The specific variables I am most interested in exploring are:

Residence(RE): Physical structure of residence; address where SP lives

Housing Type (HT): Description of type of place SP lives (including questions that trigger need for FQ administration); is place part of retirement community

Community (CM): Agreement with statements about community: know each other, willing to help, trust

Mobility Devices (MD): Compensatory Strategies Used: cane, walker, wheelchair (is it where SP lives), scooter (is it where SP lives) 
Sensory and Physical Impairments & Symptoms (SS): Impairments & Capacity Hearing; vision; chewing & swallowing; speaking & being understood; pain: limits activities, frequency of meds, location; breathing problems (limits activities); strength or movement shoulders, arms, hands, feet (limits activities); strength or movement hips, legs, knees, feet (limits activities); low energy/easily exhausted (limits activities); balance/coordination (limits activities) 

Physical Capacity (PC): Capacity Able to: walk 6 blocks/walk 3 blocks, climb 20 stairs/climb 10 stairs, lift and carry 20 lbs/10 lbs, kneel down/bend over, heavy object overhead/reach overhead, open sealed jar/grasp small objects 

Cognitive Assessments: Proxy (CP): Capacity Overall memory rating; 8 items on changes in thinking/memory; behavior: getting lost, wanders off, able to leave alone, sees/hears things 

Cognitive Assessments: Self (CG): Capacity Self-rated memory (current, interferes activities, one year ago); date (mo/day/year) and day of week; 10 word immediate recall; clock-drawing test; naming President and Vice President; 10 word delayed recall

Mobility (MO): Going outside home/building: frequency, frequency of mobility device use, help and who helps, frequency done by self, difficulty by self, unmet need for help; If multiunit: Frequency of leaving private space to go other areas in building; frequency leaving room where SP sleeps; Getting around inside home/building: frequency, frequency of mobility device use, frequency hold onto walls/furniture, help and who helps, frequency done by self, difficulty by self, frequency compared to a year ago, unmet need for help; Getting out of bed: frequency use cane/walker, help and who helps, frequency done by self; difficulty by self, unmet need for help 

Duration of Mobility Accommodations (DM): Duration of mobility help (getting outside, getting around inside, getting out of bed) and mobility device use (cane, walker, wheelchair, scooter).

Participation in Activities (PA): Visit in person with friends/family not co-resident, health/functioning keep from doing; transportation keep from doing; how important to SP; Attend religious services, health/functioning keep from doing, transportation keep from doing; how important to SP; Participate in clubs, classes, or other organized activities, health/functioning keep from doing; transportation keep from doing, how important to SP; Go out for enjoyment, health/functioning keep from doing, transportation keep from doing; how important to SP; Work for pay or in a business SP owns, health/functioning keep from doing; Do volunteer work, health/functioning keep from doing; Provide care/look after an adult or child who cannot care for themselves, who was that; Go walking for exercise; Do vigorous activities What is favorite activity, health/functioning keep from doing

### Limitations
As I explore the data I may need to trim the list of variables examined based on time, computing resources, and/or quality/completeness of the data. I will aim to explore the relationship between disability and social connectedness both longitudinally, using the re-interviews of specific individuals, and at various points in time using annual slices of the data.
