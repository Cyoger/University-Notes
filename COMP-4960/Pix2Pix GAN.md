image to image translation 
one representation to another possible representation 
we have learned loss function as well 
![[Pasted image 20231128133424.png]]

minibatch SGD and applly Adam solver, with 0.0002 learning rate and momentum beta1 = 0.5, beta2 = 0.999


discriminator architecture = PatchGAN
penalizes structure at scale of patches, this discriminator tries to classify if each NxN patch in an image is real or fake. 