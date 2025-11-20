# SUMMARY PAPERS

# Metadata
https://www.nature.com/articles/s41598-019-55977-z.pdf 

# methods
- 31 participants exp1
- 29 participants exp2
- Design: between-odour conditions (pleasant / unpleasant / neutral) × within-participant repeated trials.
- Two experiments (same task, differences only in sniff cue timing).
- Task: Go/No-Go with 5:1 or 3:1 Go/NoGo ratio.
- Odours: clean air, orange, methional, 2,4,5-trimethylthiazole (exp1) and clean air, orange and orange, hexenol, civet and clean air (exp2). 

### Power analysis: 
-	Medium effect size at power=0.90 and α=0.05 suggested a sample size of twenty-nine; slightly oversampled

### Exclusion rules:
-	RTs > 2.5 SD removed (1.8% of trials)
 
### Modelling approach:
-	LME (Gaussian): RT, pleasantness, intensity
-	GLME (binomial): failed-to-Go, failed-to-NoGo
All models include participants as random intercepts
Optimizer: bobyqa for GLME convergence issues
Fixed factors enter LME models and compared via AIC model comparison; LR tests used for p-values (likelihood ratio) 

### Fixed-effects factors:
-	For pleasantness & intensity: odour (3 levels) + cycle (ratings over time)
-	For RTs & error rates: valence (pleasant / unpleasant / control)
-	For failed-to-Go (Exp 1 only): preceding Go trial count (1, 3, 5, 7)
### Inference:
-	LR tests
-	Tukey HSD with Bonferroni correction for follow-ups: α = .05
### Reporting:
-	LME: means + SD
-	GLME: percent failed trials

#results 
## EXPERIMENT 1

### Odour pleasantness ratings
-	Main effect of odour: χ²(2) = 604.81, p < .001, AICRL > 100 
-	Effect of cycle: χ²(8) = 1.610, p = .991, AICRL < .001
-	Odour × cycle interaction: χ²(16) = 8.454, p = .934, AICRL < .001

#### Post-hoc comparisons
-	Trimethyloxazole  (29.9±24.5) vs Orange (73.3±18.1): p < .001
-	Trimethyloxazole vs Clean air (45.2±13.9): p < .001
-	Orange vs Clean air: p < .001

### Odour intensity ratings
-	Main effect of odour: χ²(2) = 933.21, p < .001, AICRL > 100
-	Effect of cycle: χ²(8) = 12.186, p = .143, AICRL = .148
-	Interaction: χ²(16) = 8.191, p = .943, AICRL < .001

#### Post-hoc comparisons
-	Orange  (62.5±24.2) vs Trimethyloxazole  (66.0±26.0): p = .067
-	Clean air  (9.4±14.6) vs Orange: p < .001
-	Clean air vs Trimethyloxazole: p < .001

### Failed-to-No-Go (response inhibition)
-	Main effect of valence: χ²(2) = 11.065, p = .004, AICRL = 34.202

#### Post-hoc comparisons
-	Pleasant (21%) vs Control (16%): p = .005
-	Pleasant vs Control (text version also lists): p = .003
-	Pleasant vs Unpleasant (19.3%): p = 1.000
-	Control vs Unpleasant: p = .065 (trend)

### Failed-to-Go (attentional failures)
-	Main effect of valence: χ²(2) = 7.812, p = .020, AICRL = 6.726

#### Post-hoc comparisons
-	Pleasant (5.3%) vs Control (6.6%): p = .021Control vs Unpleasant (5.7%): p = .142
-	Pleasant vs Unpleasant: p = 1.000

### Reaction times (Go trials)
-	Main effect of valence: χ²(2) = 191.33, p < .001, AICRL > 100

#### Post-hoc comparisons
-	Pleasant (330ms) vs Control (345ms): p < .001
-	Unpleasant (335ms) vs Control (345ms): p < .001
-	Pleasant vs Unpleasant: p < .001


##EXPERIMENT 2 

### Odour pleasantness ratings
-	Main effect of odour: χ²(2) = 251.77, p < .001, AICRL > 100
-	Effect of cycle: χ²(4) = 1.142, p = .888, AICRL = .032
-	Interaction: χ²(8) = 2.869, p = .942, AICRL = .001
#### Post-hoc comparisons
-	Hexenol vs Orange: p < .001
-	Hexenol vs Clean air: p < .001
-	Orange vs Clean air: p < .001

### Odour intensity ratings
-	Main effect of odour: χ²(2) = 448.14, p < .001, AICRL > 100
-	Effect of cycle: χ²(4) = 4.445, p = .349, AICRL = .169
-	Interaction: χ²(8) = 6.844, p = .553, AICRL = .010
#### Post-hoc comparisons
-	Orange vs Hexenol: p = .084
-	Clean air vs Orange: p < .001
-	Clean air vs Hexenol: p < .001

### Failed-to-No-Go responses
-	Main effect of valence: χ²(2) = 0.167, p = .920, AICRL = 0.147 n.s.

### Failed-to-Go responses
-	Main effect of valence: χ²(2) = 23.69, p < .001, AICRL > 100 
#### Post-hoc comparisons
-	Pleasant (3.3%) vs Control (6.5%): p < .001
-	Unpleasant (3.4%) vs Control: p < .001
-	Pleasant vs Unpleasant: p = 1.000

### Reaction times (Go trials)
-	Main effect of valence: χ²(2) = 180.3, p < .001, AICRL > 100
#### Post-hoc comparisons
-	Pleasant (330ms) vs Control (350ms): p < .001
-	Unpleasant (331ms) vs Control: p < .001
-	Pleasant vs Unpleasant: p = 1.000

#data

##Trial structure:
-	Go/NoGo, with ~3:1 Go:NoGo ratio
-	Pseudo-random with odour change constraints

##Variables:
-	RT: continuous (ms), approx Gaussian after trimming
-	Failed-to-Go: binomial (0/1)
-	Failed-to-NoGo: binomial (0/1)
-	Pleasantness/intensity: continuous VAS (0–100)
Within-subject repeated factors: odour / valence
Between-subject factors: none
- Exp1: 8 blocks, 100 trials each (25 per odour condition) 5:1 Go/No-go ratio
- Exp2: 4 blocks, 80 trials each (20 per odour condition) 3:1 Go/No-go ratio

