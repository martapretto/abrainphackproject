# Metadata

https://journals.sagepub.com/doi/full/10.1177/0956797621993111


# Methods
- participants n = 36
- linear mixed-effects models using the R package lme4
- conditions: writing, typing, visual 
    (these are the learning conditions between the pre- and post-tests, between-subjects)
- task: forced-choice between a pair of arabic letter for recognition
- pre and post tests after learning
- number of learning session (covariate) varies among subjects

## Models 
1. letter naming:
- log(RT) ~ Condition + Days-to-Post + Number of Sessions + Previous Trial RT + Recognition Accuracy + Recognition RT + (1 + Recognition Accuracy + Recognition RT + Previous Trial RT | participant) + (1 | stimulus)
- Accuracy ~ Condition + Days-to-Post + Number of Sessions + Recognition Accuracy + Recognition RT + (1 + Recognition Accuracy + Recognition RT | participant) + (1 | stimulus)
2. letter writing:
- Accuracy ~ Condition + Days-to-Post + Number of Sessions + Recognition Accuracy + Recognition RT + (1 + Recognition Accuracy + Recognition RT | participant) + (1 | stimulus)
3. spelling to dictation:
- Accuracy ~ Condition + Length + Familiarity + Number of Sessions + Days-to-Post + (1 + Length + Familiarity | participant) + (1 | stimulus)
4. reading words:
- Accuracy ~ Condition + Length + Familiarity + Number of Sessions + Days-to-Post + (1 + Length + Familiarity | participant) + (1 | stimulus)
5. letter recognition (no sig, therefore descriptive not reported):
- log(RT) ~ Condition + First Attempt + Days-to-Post + Number of Sessions + Previous Trial RT + (1 + First Attempt + Previous Trial RT | participant) + (1 | stimulus)
- Accuracy ~ Condition + First Attempt + Days-to-Post + Number of Sessions + (1 + First Attempt | participant) + (1 | stimulus)
- w (writing condition) is the reference intercept and other two t and v are dummy coded

# Results
- they are only interested in the difference between the 3 conditions (two-way interaction)
3, p < 0.05
1, p < 0.001

# Data
training sessions (number of sessions)
- writing condition (M = 3.67 sessions, SE = 0.36),
- typing condition (M = 3.92, SE = 0.38)
- visual condition (M = 4.25, SE = 0.37)


1) letter naming:
Mean RT with correct responses
- typing: 1,545 ms (SD = 337)
- visual: 1,393 ms (SD = 368)
- writing: 1,308 ms (SD = 235)

There was a significant difference between the typing and writing conditions (p < .05);
The total model R2 was 43%

2) letter writing:
Mean accuracy
- typing: 78.5% (SD = 15.3%)
- visual: 64.5% (SD = 23.8%)
- writing: 91.0% (SD = 7.2%)

There was a nonsignificant trend of higher accuracy in the writing condition compared with the typing condition (p < .09) and a significant effect of higher accuracy in the writing condition compared with the visual condition (p < .001).

The total model R2 was 46%.

3) spelling to dictation:
Mean accuracy
- typing: 62.3% (SD = 15.4%)
- visual: 72.0% (SD = 25.2%)
- writing: 76.3% (SD = 14.5%)

There was no effect of familiarity (previously trained words vs. novel words), p > .1. Accuracy in word spelling was significantly higher in the writing than in the typing condition (p < .05), and there was no significant difference in accuracy between the visual and writing conditions.

The total model R2 was 38%.

4) reading words:
Mean accuracy
- typing: 50.8% (SD = 28.5%)
- visual: 59.2% (SD = 33.4%)
- writing: 66.6% (SD = 22.0%)

There was no effect of familiarity (previously trained words vs. novel words), p > .1. Partici-
pants in the writing condition were not significantly more accurate than those in either the typing or the visual conditions (p ≈ .18 and .47, respectively).

The total model R2 was 57%.


