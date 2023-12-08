---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---
<img src="/images/banner6.png" style="pointer-events: none; user-select: none;">
<p>
The third version of the Efficient Natural Language and Speech Processing (ENLSP-III) workshop will focus on the future of large language models and their emerging applications on different domains such as natural language, speech processing, and biological sequences; and the target is on how to make them more efficient in terms of <b>Data</b>, <b>Model</b>, <b>Training</b>, and <b>Inference</b> for real-world applications as well as academic research.  The workshop program offers an interactive platform for gathering different experts and talents from academia and industry through invited talks, panel discussion, paper submissions, reviews, interactive posters, oral presentations and a mentorship program.
This will be a unique opportunity to discuss and share challenging problems, build connections,  exchange ideas and brainstorm solutions, and foster future collaborations. The topics of this workshop can be of interest for people working on general machine learning, deep learning, optimization, theory and NLP & Speech applications. 
</p>


<h2 class="blackpar_title" id="overview">Overview</h2>
<p>
With the emergence of large language and speech models (such as GPT-3, GPT-4, wav2vec, Hubert, wavLM, Whisper, PALM, LLaMA, and PALM 2) and then their variants which are fine-tuned on following instructions (such as Instruct-GPT, Alpaca, Dolly) and especially, conversational language models (such as ChatGPT, Bard, Vicuna, StableLM-Tuned, OpenAssistant), we have taken one significant step towards mimicking the human intelligence by machines. The contributions of Language models did not even stop at this level, their emerging usage in biological (protein language models such as protTrans models, ESM, protGPT2) and chemical domains (small molecule and polymer language models like SMILESBERT, polyBERT, and transPolymers) have further expanded their applications across various scientific disciplines. As a result, these models are revolutionizing the way we approach research and knowledge discovery, paving the way for more innovative breakthroughs in diverse fields.

This great success has come with the price of pre-training these large models on a huge amount of data, fine-tuning them with instruction-based data and human supervised fine-tuning data, and extensive engineering efforts. Despite the great success of these large models, it is evident that most of them are largely over-parameterized and their efficiency is under question. Lack of efficiency can largely limit the application of these advanced techniques in practice. Training, adapting or deploying these large models on devices or even cloud services with limited memory and computational power can be very challenging.
<br><br>
While these current achievements have paved the road for the faster progress of improving large foundation models from different aspects in the future, we need to address different efficiency issues of these models at the same time. For example, in natural language, it has been shown that larger model sizes reveal more zero-shot or few-shot (in-context learning) capabilities in handling different tasks. However, collecting data, pre-training and maintaining such large models can be very expensive. In terms of training data, it is still not very clear to what extent expanding the training data can improve these pre-trained models and whether we can compress pre-training data without much sacrificing the performance. The problem of efficiency becomes more critical when we think about pre-training multimodal models.  At the time of deployment, designing proper prompts for different tasks can be very arbitrary and time consuming. Fine-tuning large language models with billions of parameters is very costly. One can think of transferring the knowledge of large foundation models to smaller models (by distillation or symbolic distillation) but still we do not have a straightforward recipe for this task. Furthermore, there is a debate in the literature that to what extent we can transfer the knowledge of powerful large black-box models such as ChatGPT to smaller models in specific or general domains. Additionally, due to the huge size of the foundation models, applying model compression techniques to them is not an easy task. 

In the light of advances in large protein language models and their application in biology, this year there will be a special track focused on emerging protein language models, their pretraining, fine tuning, applications, and approaches for improving their efficiency. 
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
<b>Special track: Protein Language Models </b> Emergence and the future of language models for biological sequences and how to make them more efficient.
<ul>
	<li>Protein language models and their applications</li>
	<li>Refining the pretraining algorithm and/or model architecture of LLMs to optimize performance in the protein domain.</li>
	<li>Optimizing the curriculum learning (order of pretraining data presentation) for more efficient pre-training or fine tuning of protein language models</li>
	<li>Efficient remote homology via dense retrieval using protein language models</li>
	<li>Combining sequence and 3D structure in pretraining or fine-tuning of the models</li>
	<li>Multi-modal language models for biological sequences.</li>
</ul>
<b>Other Efficient Applications</b>
<ul>
	<li>Knowledge localization, knowledge editing, or targeted editing/training of foundation models</li>
	<li>Efficient dense retrieval and search</li>
	<li>Efficient graphs for NLP</li>
	<li>Training models on device</li>
	<li>Incorporating external knowledge into pre-trained models</li>
	<li>Efficient Federated learning for NLP: reduce the communication costs, tackling heterogeneous data, heterogeneous models.</li>
</ul>

</p>

<h2 class="blackpar_title">Submission Instructions</h2>
<p>
You are invited to submit your papers in our CMT submission portal <a href="https://cmt3.research.microsoft.com/ENLSP2023">(Link)</a>. All the submitted papers have to be anonymous for double-blind review. We expect each paper will be reviewed by at least three reviewers. The content of the paper (excluding the references and supplementary materials) should not be longer than 4 pages, strictly following the NeurIPS template style. 
<br /><br />
Authors can submit up to 100 MB of supplementary materials separately. Authors are highly encouraged to submit their codes for reproducibility purposes. According to the guideline of the NeurIPS workshops, already published papers are not encouraged for submission, but you are allowed to submit your ArXiv papers or the ones which are under submission. Moreover, a work that is presented at the main NeurIPS conference should not appear in a workshop. Please make sure to indicate the complete list of conflict of interests for all the authors of your paper. To encourage higher quality submissions, our sponsors are offering the <b>Best Paper</b> and the <b>Best Poster</b> Award to qualified outstanding original oral and poster presentations (upon nomination of the reviewers). Also, we will give one outstanding paper certification for our special track of protein language models. Bear in mind that our workshop is not archival, but the accepted papers will be hosted on the workshop website.
</p>

<h2 class="blackpar_title">Important Dates:</h2>
<p>
<ul>
	<li>Submission Deadline: October 2, 2023 <b>AOE</b> </li>
	<li>Acceptance Notification: October 27, 2023 <b>AOE</b> </li>
	<li>Camera-Ready Submission: November 3, 2023 <b>AOE</b> </li>
	<li>Workshop Date: <b>December 16, 2023 </b></li>
</ul>
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
<h2 class="blackpar_title" id="schedule">Schedule</h2>
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
	<div class="card_perso column_perso justify-content-center" id="volunteer_card">
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

<h2 class="blackpar_title">Diamond Sponsors</h2>
<!-- <center>
	<img src="/images/logos.png">	
	<img src="/images/BASF_logo.png">	
</center> -->
<div class="row">
	<div class="col">
		<center>
			<img src="/images/huawei_logo.png" width="400px">
		</center>
	</div>
	<div class="col">
		<center>
			<img src="/images/BASF_logo.png" width="400px">
		</center>
	</div>
</div>
<br><br>
<h2 class="blackpar_title">Platinum Sponsor</h2>
<div class="row">
	<div class="col">
		<center>
			<img src="/images/netmind_logo.png" width="400px">
		</center>
	</div>
</div>
<br><br>
<h2 class="blackpar_title">Gold Sponsor</h2>
<div class="row">
	<div class="col">
		<center>
			<img src="/images/Apple-Logo.jpg" width="200px">
		</center>
	</div>
</div>
