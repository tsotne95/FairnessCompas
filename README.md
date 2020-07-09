# Fairness classifier for Compas dataset

Accorrding data Black defendants are 44% more likely than white defendants to receive a higher score correcting for the seriousness of their crime, previous arrests, and future criminal behavior.

So, for the new classifier used two different threshold.

In this case raised the threshold for blacks from 0.5 to 0.7, and reduced threshold from 0.5 to 0.495 for whites, which equalizes the FPR at about 17%.

The overall accuracy fell only slightly from 67% to 65%, and the accuracy for black defendants fell from 66% to 64%, for white defendants it's same 66%.

But the PPV for blacks defendants, the probability that someone who is categorized as high risk will actually be re-arrested within two years, increased from 69% to 74%, because the higher threshold removes some of the people who were not particularly risky from the high risk group. The cost is a higher false negative rate for blacks, which changed from 33% to 52%.
