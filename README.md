# Simulating Game Player

Problem settings: Bots are easy to detect due to stereotype movements e.g., predefined coordinates (X,Y)

Aim: simulate the movements of game players to make bots move or walk like humans.

Train sequences of moves

Predict next moves

# Model
LSTM, train sequences of moves

# Data
Scrape behaviors from the gaming forum, "move to loc" scripts
AND use pre-determined bot scripts

# Input
[[X1,Y1],[X2,Y2],[X3,Y3]]

# Output
[[X4,Y4]]

# Evaluate

Results:
-        -PREDICT                   -ACTUAL
move 1 [ 85941.016 132009.2  ] ['82861', ' 148330']

move 2 [ 85845.72 132180.05] ['82801', ' 149368']

move 3 [ 85836.29 132635.95] ['81572', ' 149466']

move 4 [ 85384.33 133029.98] ['81331', ' 149685']

move 5 [ 84900.375 133140.39 ] ['81331', ' 149685']

move 6 [ 26151.623 164524.36 ] ['20467', ' 187061']

move 7 [ 25944.8 163758.3] ['19703', ' 185483']

move 8 [ 25547.104 162507.28 ] ['20896', ' 184693']

move 9 [ 25667.293 161352.3  ] ['20896', ' 184693']

move 10 [117203.83 193819.92] ['111364', ' 219123']

move 11 [117162.38 193727.06] ['110271', ' 219030']

move 12 [116812.2 193655.7] ['110075', ' 218989']

move 13 [116416.46 193444.73] ['110080', ' 217990']

move 14 [115993.15 192958.42] ['110032', ' 217279']

move 15 [115801.56 192388.67] ['108880', ' 217539']

move 16 [115522.29 192184.67] ['107862', ' 217546']

move 17 [114909.22 192039.25] ['107123', ' 218150']

move 18 [114223.25 192170.61] ['107122', ' 217833']

move 19 [113764.64 192081.23] ['107110', ' 217123']

move 20 [113459.62 191770.28] ['107110', ' 217123']

Predicted moves align quite well with actual moves.

For instance, moves 8 and 9 indicate a player did not move but stayed still in those coordinates. LSTM model could maintain similar moves with actual moves, although the predicted moves were completely novel.
