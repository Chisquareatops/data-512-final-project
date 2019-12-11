# Final Project Proposal

## Background

### Related Work
The relationship between disability and social engagement has been well studied from a number of angles, but given the extremely multifaceted nature of human social relationships and psychological well-being, and therefore the extremely high number of variables involved in examining these parts of the human experience, there is still a signifigant need to improve our understanding.

It is well established in the current body of research that social engagement is strongly and negatively correlated with physical and cognitive disability among older adults, and that this relationship exists even when controlling for other important factors including socioeconomic status, gender, and race (Mendes de Leon, Glass, & Berkman, 2003, Bath & Deeg, 2005, Keeney & Jette, 2019). Although this area is generally well-studied, many of the existing studies did not consider longitudinal data or were able to obtain longitudinal data for relatively small numbers of individuals; some of the longitudinal research that does exist suggests a weakening of the protective effect of social engagement against disability over time (Mendes de Leon et al., 2003). There has also been significant inconsistency in how terminology surrounding “social engagement” has been used, and there has been a major division between research focusing on participation in social activities and research focusing on social networks (Andersson 1998; Bennett 2002). The extremely rich dataset we propose to use here offers a number of variables that address both fundamental approaches to social engagement.

### Purpose of Proposed Project
This project aims to use longitudinal data for over 5,000 individuals to examine the relationships between various types of social engagement and several kinds of disability over either 8 or 4 years. The dataset being explored for this project also contains more markers of social engagement than do the majority of existing papers, creating the opportunity for more detailed insights.

This work aims to help highlight the most fruitful avenues for preventing or slowing increased disability among aging adults by highlighting the most important protective factors. The primary audience will be researchers and service providers working in elder care.

### Hypotheses
The primary hypothesis under investigation is that increasing levels of disability, especially cognitive impairment, will correlate with decreasing levels of participation in valued activities and a narrowing of the social circle. This hypothesis is strongly informed by (and consistent with) the conclusions of prior research.

A secondary hypothesis is that this association will be less pronounced in individuals who are able to age in place (i.e. remain in their homes). This secondary hypothesis was informed by prior research that suggests aging in place is associated with lower levels of disability and higher levels of social engagement (Aliberti & Covinsky, 2019, Low, 2018).

## Data

### Summary
The proposed project will use the National Health and Aging Trends Study (NHATS) dataset; specifically the final release of rounds one through eight. This dataset contains information from a nationally representative sample of Medicare beneficiaries aged 65 or older. The first sample was interviewed in 2011 and there have been annual follow up interviews, with a replenishment of participants in 2015. An incredible amount of information is gathered from these individuals and other individuals in their social networks; the proposed project is particularly concerned with variables related to social engagement and various disabilities, both physical and cognitive. 

The data contained in NHATS is not just survey data, but also includes data gathered from performance based tests of physical and cognitive capacity (about which perceptual, self-rated information is also gathered).

### Files
This data is contained primarily in the following files:

NHATS_Round_8_SP_File.dta contains the sample person (SP) and the facility questionnaire (FQ) data (5,547 observations and 1,317 variables).

NHATS_Round_8_OP_File.dta contains the other person (OP) data (46,905 observations and 571 variables).

NHATS_Round_8_Tracker_File.dta contains tracking information for all persons sampled for NHATS (19,530 observations and 889 variables).

This data is publically available from https://www.nhats.org. Registration is required to access the data files.

### Variables Under Consideration
The NHATS R8 Final Crosswalk between Instruments and Codebook, found on the NHATS website linked above, is 98 pages long. The user guide, which contains more thorough explanations of each field, is 147 pages long. Not every measure has been considered for this project, and not all measures considered have yet been examined. However, a preliminary list of target variables has been identified as possible independent or dependent variables for the proposed analysis:

Residence(RE): Physical structure of residence; address where SP lives

Housing Type (HT): Description of type of place SP lives (including questions that trigger need for FQ administration); is place part of retirement community

Community (CM): Agreement with statements about community: know each other, willing to help, trust

Mobility Devices (MD): Compensatory Strategies Used: cane, walker, wheelchair (is it where SP lives), scooter (is it where SP lives) Sensory and Physical Impairments & Symptoms (SS): Impairments & Capacity Hearing; vision; chewing & swallowing; speaking & being understood; pain: limits activities, frequency of meds, location; breathing problems (limits activities); strength or movement shoulders, arms, hands, feet (limits activities); strength or movement hips, legs, knees, feet (limits activities); low energy/easily exhausted (limits activities); balance/coordination (limits activities)

Physical Capacity (PC): Capacity Able to: walk 6 blocks/walk 3 blocks, climb 20 stairs/climb 10 stairs, lift and carry 20 lbs/10 lbs, kneel down/bend over, heavy object overhead/reach overhead, open sealed jar/grasp small objects

Cognitive Assessments: Proxy (CP): Capacity Overall memory rating; 8 items on changes in thinking/memory; behavior: getting lost, wanders off, able to leave alone, sees/hears things

Cognitive Assessments: Self (CG): Capacity Self-rated memory (current, interferes activities, one year ago); date (mo/day/year) and day of week; 10 word immediate recall; clock-drawing test; naming President and Vice President; 10 word delayed recall

Mobility (MO): Going outside home/building: frequency, frequency of mobility device use, help and who helps, frequency done by self, difficulty by self, unmet need for help; If multiunit: Frequency of leaving private space to go other areas in building; frequency leaving room where SP sleeps; Getting around inside home/building: frequency, frequency of mobility device use, frequency hold onto walls/furniture, help and who helps, frequency done by self, difficulty by self, frequency compared to a year ago, unmet need for help; Getting out of bed: frequency use cane/walker, help and who helps, frequency done by self; difficulty by self, unmet need for help

Duration of Mobility Accommodations (DM): Duration of mobility help (getting outside, getting around inside, getting out of bed) and mobility device use (cane, walker, wheelchair, scooter).

Participation in Activities (PA): Visit in person with friends/family not co-resident, health/functioning keep from doing; transportation keep from doing; how important to SP; Attend religious services, health/functioning keep from doing, transportation keep from doing; how important to SP; Participate in clubs, classes, or other organized activities, health/functioning keep from doing; transportation keep from doing, how important to SP; Go out for enjoyment, health/functioning keep from doing, transportation keep from doing; how important to SP; Work for pay or in a business SP owns, health/functioning keep from doing; Do volunteer work, health/functioning keep from doing; Provide care/look after an adult or child who cannot care for themselves, who was that; Go walking for exercise; Do vigorous activities What is favorite activity, health/functioning keep from doing

Number in Social Network (SN), a derived variable expressing how many people are in the studied individual’s social network.

SP Has No One to Talk To (SN), a flag variable identifying studied individuals who have no one to talk to.

## Methodology
The primary methodology will be a series of multiple linear regressions, investigating the ability of various social-engagement measures (and their interactions) to predict each of several measures of disability. This approach has been strongly informed by a number of past studies which suggest the relationship between social engagement and disability may be fundamentally linear (Mendes de Leon et al., 2003, Hreha et al., 2019) as well as early visual inspections of the data. Some past research has used logistic regression models, but this approach is not appropriate here because the current project concerns disability-related outcomes that must be measured continuously (e.g., mobility, cognitive function).

This approach is appropriate because the proposed project concerns many continuous independent variables. Although we are interested in a few different dependent variables (disability), each of which are continuous, we want to treat them separately because we are not examining the ways different physical disabilities are related to each other or to cognitive disability. This approach will highlight important protective factors for specific, identifiable types of disability, which will lead to actionable plans for populations who have or are at risk for one of these types of disability.

## Works Cited
Adersson, L., (1998). Loneliness research and interventions: A review of the literature, Aging & Mental Health, 2:4, 264-274, DOI: 10.1080/13607869856506

Aliberti, M. J. R., & Covinsky, K. E., (2019). Home modifications to reduce disability in older adults with functional disability. JAMA Internal Medicine, 179(2), 211–212. DOI: 10.1001/jamainternmed.2018.6414

Bath, P. A., & Deeg, D., (2005). Social engagement and health outcomes among older people: Introduction to a special section. European Journal of Ageing, 2(1), 24–30. DOI:
10.1007/s10433-005-0019-4

Bennett, (2002). Low level social engagement as a precursor of mortality among people in later life. Age and Ageing, 31(3), 165–168. DOI: 10.1093/ageing/31.3.165

Hreha, Kimberly P., Smith, Amanda E., Wong, Jennifer L., Mroz, Tracy M., Fogelberg, Donald J. & Molton, Ivan., (2019). Impact of secondary health conditions on social role participation for a long-term physical disability cohort. Psychology, Health & Medicine, 24(10), 1159-1170. DOI: 10.1080/13548506.2019.1595684

Keeney, T., & Jette, A. M., (2019). Individual and environmental determinants of late-life community disability for persons aging with cardiovascular disease. American Journal of Physical Medicine & Rehabilitation, 98(1), 30–34. ISSN: 0894-9115 

Low, Jennifer., (2018). We're still here: The implications of aging with a disability. Creative Components. 83. Retrieved from https://lib.dr.iastate.edu/creativecomponents/83

Mendes de Leon, C. S., Glass, T. A., & Berkman, L. F., (2003). Social engagement and disability in a community population of older adults: the New Haven EPESE. American Journal of Epidemiology, 157(7), 633–642., ISSN: 0002-9262
