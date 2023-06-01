---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---
<div style="font-family: 'Source Sans Pro', sans-serif; background: url('/images/banner_no_text.png') no-repeat; background-size: cover; user-select: none;">
	<center>
		<h2 class="blackpar_title" >The 3<sup>rd</sup> workshop on<br>Efficient Natural Language and Speech Processing (ENLSP)</h2>
		<h3 class="blackpar_title">The Future of Large Language and Speech Foundation Models</h3>
		<h3 class="blackpar_title">[DATE TBD], New Orleans  <b>-</b> In person </h3>
	</center>
</div>

<p>
The third version of the Efficient Natural Language and Speech Processing (ENLSP-III) workshop will focus on the future of large language and speech foundation models; and how to make them more efficient in terms of <b>Data</b>, <b>Model</b>, <b>Training</b>, and <b>Inference</b> for real-world applications as well as academic research.  The workshop program offers an interactive platform for gathering different experts and talents from academia and industry through invited talks, panel discussion, paper submissions, reviews, interactive posters, oral presentations and a mentorship program.
This will be a unique opportunity to discuss and share challenging problems, build connections,  exchange ideas and brainstorm solutions, and foster future collaborations. The topics of this workshop can be of interest for people working on general machine learning, deep learning, optimization, theory and NLP & Speech applications. 
</p>


<h2 class="blackpar_title" id="overview">Overview</h2>
<p>
With the emergence of large language and speech models (such as GPT-3, GPT-4, wav2vec, Hubert, wavLM, Whisper, PALM, LLaMA, and PALM 2, and then their variants which are fine-tuned on following instructions (such as Instruct-GPT, Alpaca, Dolly and especially, conversational language models (such as ChatGPT (Link), Bard, Vicuna, StableLM-Tuned, OpenAssistant), we have taken one significant step towards mimicking the human intelligence by machines. This great success has come with the price of pre-training these large models on a huge amount of data, fine-tuning them with instruction-based data and human supervised fine-tuning data, and extensive engineering efforts. Despite the great success of these large models, it is evident that most of them are largely over-parameterized and their efficiency is under question. Lack of efficiency can largely limit the application of these advanced techniques in practice. Training, adapting or deploying these large models on devices or even cloud services with limited memory and computational power can be very challenging.
<br><br>
While these current achievements have paved the road for the faster progress of improving large foundation models from different aspects in the future, we need to address different efficiency issues of these models at the same time. For example, it has been shown that larger model sizes reveal more zero-shot or few-shot (in-context learning) capabilities in handling different tasks. However, collecting data, pre-training and maintaining such large models can be very expensive. In terms of training data, it is still not very clear to what extent expanding the training data can improve these pre-trained models and whether we can compress pre-training data without much sacrificing the performance. The problem of efficiency becomes more critical when we think about pre-training multimodal models.  At the time of deployment, designing proper prompts for different tasks can be very arbitrary and time consuming. Fine-tuning large language models with billions of parameters is very costly. One can think of transferring the knowledge of large foundation models to smaller models (by distillation or symbolic distillation) but still we do not have a straightforward recipe for this task. Furthermore, there is a debate in the literature that to what extent we can transfer the knowledge of powerful large black-box models such as ChatGPT to smaller models in specific or general domains. Additionally, due to the huge size of the foundation models, applying model compression techniques to them is not an easy task. 
</p>

<!-- Call for Papers -->
<h2 class="blackpar_title" id="call_for_papers">Call for Papers</h2>
<p>
It is of vital importance to invest on future of large foundation models by enhancing their efficiency in terms of data, modeling, training and inference from different perspectives highlighted in the workshop.  In this regard, we share some active research topics in this domain which might be of interest to the NeurIPS community to get their participation, ideas and contributions.  The scope of this workshop includes, but not limited to, the following topics:
<br><br>
<b>Efficient Pre-Training</b> How can we reduce the cost of pre-training new models?
<ul>
	<li>Accelerating the pre-training process</li>
	<li>Efficient initialization and hyper-parameter tuning (HPT)</li>
	<li>Data vs. scale of pre-trained models</li>
	<li>Efficient Multimodal (e.g., text–speech) pre-trained models and efficiency issues related to it</li>
	<li>New efficient architectures (e.g. using sparse structures or mixture of experts (MoEs)) or new training objectives for pre-trained models</li>
</ul>
<b>Efficient Fine-tuning</b> Fine-tuning the entire parameters of large pre-trained models on downstream
tasks can be expensive and it is prone to overfitting.
<ul>	
	<li>Efficient prompt engineering and in-context learning</li>
	<li>Parameter-efficient tuning solutions (i.e. training only a portion of the entire network)</li>
	<li>Accelerating the fine-tuning process (e.g. by improving the optimizer, and layer-skipping)</li>
</ul>
<b>Data Efficiency</b> Pre-training (with unlabeled data) and fine-tuning (with labeled data) are both data hungry processes. Labeling data and incorporating human annotated data or human feedback are very time consuming and costly. Here we would like to address "how to reduced the costs borne by data?"
<ul>
	<li>Sample efficient training, training with less data, few-shot and zero-shot learning</li>
	<li>How to reduce the requirements for human labeled data?</li>
	<li>Can we rely on machine generated data for training models? (e.g. data collected from ChatGPT)</li>
	<li>Data compression, data distillation</li>
</ul>
<b>Efficient Deployment</b> How can we reduce the inference time or memory footprint of a trained model for a particular task?
<ul>
	<li>Relying on in-context learning and prompt engineering of large language models or fine-tuning smaller models (by knowledge transfer from larger models)?</li>
	<li>Neural model compression techniques such as (post-training) quantization, pruning, layer decom- position and knowledge distillation (KD) for NLP and Speech</li>
	<li>Impact of different efficient deployment solutions on the inductive biases learned by the original models (such as OOD generalization, in-context learning, in-domain performance, hallucination).</li>
</ul>
<b>Other Efficient Applications</b>
<ul>
	<li>Knowledge localization, knowledge editing, or targeted editing/training of foundation models</li>
	<li>Efficient dense retrieval and search</li>
	<li>Training models on device</li>
	<li>Incorporating external knowledge into pre-trained models</li>
	<li>Efficient Federated learning for NLP: reduce the communication costs, tackling heterogeneous data, heterogeneous models.</li>
</ul>

</p>

<h2 class="blackpar_title">Submission Instructions</h2>
<p>
TBD
</p>

<h2 class="blackpar_title">Important Dates:</h2>
<p>
TBD
</p>


<!--Confirmed Speakers-->
<h2 class="blackpar_title" id="speakers">Confirmed Keynote Speakers</h2>
<p>
{% include speakers.html %}
</p>

<h2 class="blackpar_title" id="speakers">Panelists</h2>
<p>
{% include panelists.html %}
</p>

<!-- Schedule -->
<h2 class="blackpar_title" id="schedule">Schedule (EST time zone - New York/Montreal/Toronto)</h2>
<p>
{% include schedule.html %}
</p>

<!-- Organizers -->
<h2 class="blackpar_title" id="organizers">Organizers</h2>
<p>
{% include organizers.html %}
</p>

<h2 class="blackpar_title" id="Organizers">Volunteers</h2>
<div class="row_perso">
	<div class="card_perso column_perso justify-content-center" style="margin-left:35%;">
	  <img src="/images/khalil_bibi.png" alt="Khalil Bibi" class="img_card_perso">
	  <div class="container_perso" >
		<center>
		<h6>
			<b>Khalil Bibi</b>
			<br>
			Huawei Noah's Ark Lab
			<br>
			<a href="https://scholar.google.ca/citations?user=feQAvxoAAAAJ&hl=en">
				<i class="bi bi-mortarboard-fill" style="font-size: 2rem;"></i>
			</a>
			&nbsp;
			<a href="https://www.linkedin.com/in/khalilbibi/">
				<i class="bi bi-linkedin" style="font-size: 2rem;"></i>
			</a>
		</h6>
		</center>
	  </div>
	</div>
</div>


<br><br>

<!-- Technical Committee -->
<h2 class="blackpar_title" id="technical_committee">Technical Committee</h2>
<p>
{% include technical_committee.html %}
</p>
<br><br>

<h2 class="blackpar_title">Sponsor</h2>
<center>
	<img src="/images/logos.png">	
</center>