Our ultimate goal for this Deep Learning Project was to utilize both the
SportVU dataset [1] which contains positional data for NBA players on a 2D plane
for the 2015-2016 season and a Basketball-Reference statistical dataset [4], the
corresponding players’ NBA game statistics, to determine the probability that a
given three-point shot was made. To do this, we leveraged the aforementioned
datasets as well as other sources containing play-by-play data [3] to create our own
dataset, with each datapoint consisting of 10 frames (1 second = 1 frame) before
a shot was attempted. Each frame contained the corresponding relative player
distances, offensive statistics (for each player on offense on the court for that play),
and defensive statistics (for each player on defense on the court for that play). We
furthermore evaluate the efficacy of three deep learning architectures: Recurrent
Neural Networks, Gated Recurrent Units, and Long Short Term Memory models
on our curated dataset, and surpass all current benchmarks for this task. Following
the completion of our model, we explore different real-world avenues where our
model could be applied. First, we see that we can display the names of key players
on the court by mapping the SportVU dataset to broadcast footage, and can display
whether the shot will go in or not on the given frame. This will aid novice viewers
in learning what possessions are good, and who are good three-point shooters.
Another avenue we explore is by generalizing this model to work on all basketball
game footage, done by translating the player positions from the broadcast footage
to the SportVU coordinate system and then feeding it into our model, presenting a
pipeline to encourage future researchers to tackle this task. Thus, we developed a
system to successfully classify whether a given NBA three-pointer would result in
a made or missed basket, and discuss real-world applications and generalizations.
36th Conference on Neural Information Processing Systems (NeurIPS 2022).
