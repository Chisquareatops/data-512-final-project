# National Health and Aging Trends: Disability and Social Engagement

## Background

### Related Work
The relationship between disability and social engagement has been well studied from a number of angles, but given the extremely multifaceted nature of human social relationships and psychological well-being, and therefore the extremely high number of variables involved in examining these parts of the human experience, there is still a signifigant need to improve our understanding.

It is well established in the current body of research that social engagement is strongly and negatively correlated with physical and cognitive disability among older adults, and that this relationship exists even when controlling for other important factors including socioeconomic status, gender, and race (Mendes de Leon, Glass, & Berkman, 2003, Bath & Deeg, 2005, Keeney & Jette, 2019). Although this area is generally well-studied, many of the existing studies did not consider longitudinal data or were able to obtain longitudinal data for relatively small numbers of individuals; some of the longitudinal research that does exist suggests a weakening of the protective effect of social engagement against disability over time (Mendes de Leon et al., 2003). There has also been significant inconsistency in how terminology surrounding “social engagement” has been used, and there has been a major division between research focusing on participation in social activities and research focusing on social networks (Andersson 1998; Bennett 2002). The extremely rich dataset used here offers a number of variables that address both fundamental approaches to social engagement.

### Purpose of Proposed Project
This work aims to help highlight the most fruitful avenues for preventing or slowing increased disability among aging adults by highlighting the most important protective factors. The primary audiences are researchers and service providers working in elder care.

### Hypotheses
The primary hypothesis under investigation is that increasing levels of disability, especially cognitive impairment, will correlate with decreasing levels of participation in valued activities and a narrowing of the social circle. This hypothesis is strongly informed by (and consistent with) the conclusions of prior research.

## Data

### Modifications to the Original Data

The National Health and Aging Trends Study (NHATS) has made a huge dataset available to the public. However, using this data requires registering through www.nhats.org and agreeing to the NHATS Conditions of Use (found here: https://www.nhatsdata.org/Home/CondOfUse).

These conditions prohibit sharing the NHATS data publically. In order to comply, this repository contains a subset of the NHATS data that has been altered in several ways:

1. The data subset contains only 40 out of the originally thousands of columns.
2. All of the variables have been re-named.
3. Noise has been added to the variables where this is possible.
4. In the original data, different reasons for missing values are coded with different indicators; in the data in this repository, all missing values are coded as -1.
5. The original data was slightly oversampled so that there is not a 1:1 correspondence between rows in this dataset and rows in the original dataset.
6. Some categorical variables have been recoded as binary variables, indicating the presence or absence of one category.
7. All rows in this dataset have been assigned a new id variable which is unrelated to the id variable in the original data set.

It is likely that even with all of these adjustmets, the data contained in this repository could be reconnected to the original data with some degree of accuracy. However, the original data has been anonymized by NHATS and contains no personally identifiable information. NHATS wants users to obtain their data through the NHATS website so that they can know who is using the dataset. The data has been altered in order to create a reproducible project while not violating the NHATS Conditions of Use.

I strongly encourage everyone to visit www.nhats.org to register and download the original data. It is a rich and valuable source of information.

The analyses contained in this repository were performed first on the actual data and then on the altered subset offered here to confirm that the relevant coefficients, P-values, R-squared values, etc. are extremely close.

### Summary
This project uses a slightly altered subset of the National Health and Aging Trends Study (NHATS) dataset; specifically the final release of rounds one through eight. This dataset contains information from a nationally representative sample of Medicare beneficiaries aged 65 or older. The first sample was interviewed in 2011 and there have been annual follow up interviews, with a replenishment of participants in 2015. An incredible amount of information is gathered from these individuals and other individuals in their social networks; the proposed project is particularly concerned with variables related to social engagement and various disabilities, both physical and cognitive.

The data contained in NHATS is not just survey data, but also includes data gathered from performance based tests of physical and cognitive capacity (about which perceptual, self-rated information is also gathered).


## Methodology
The primary methodology is a series of multiple linear regressions, investigating the ability of various measures of disability (and their interactions) to predict each of several measures of social engagement. This approach has been strongly informed by a number of past studies which suggest the relationship between social engagement and disability may be fundamentally linear (Mendes de Leon et al., 2003, Hreha et al., 2019) as well as early visual inspections of the data. Some past research has used logistic regression models, but this approach is not appropriate here because the current project concerns disability-related outcomes that must be measured continuously (e.g., mobility, cognitive function).

Several multiple linear regressions are also used to investigate the relationships between several measures of social engagement, and the relationship between disability, social engagement, and general mental well-being.

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
