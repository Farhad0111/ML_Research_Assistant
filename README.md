Questions:


Convert the full repository into tensorflow, for both links.

1. Comment every function, write down what's your understanding.  If you
can translate, you do can write up a few lines.

2. Print the model summary in both pytorch and tensorflow to validate
conversion process by checking exact number of parameters for the same
model with both frameworks.

3. Print the summary for all models....from tiny to large.

4. After translation, import pytorch pretrained weight into the
tensorflow model. For sanity check,  take an image and perform inference
on that images for both models. If the decision from models align, you
know you are correct.
Do it same for the video model.

5. While translation, you might see some functions are not needed to
translate and others must. Example,  you do have to translate by
exploring this transforms function...
from torchvision import transforms

But you dont have to do this create_model...

from timm.models import create_model
