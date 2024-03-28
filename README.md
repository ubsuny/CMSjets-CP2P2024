# This is the project dealing with jets from CMS

The LHC collides protons containing colored partons: quarks, antiquarks & gluons.
The dominant hard collision process is simple 2 to 2 scattering of partons off partons via the strong color force (QCD). Each final state parton becomes a jet of observable particles. The process is called dijet production. In CMS trigger, a jet is the sum of particle 4-vectors in a cone of radius R=√(Δη^2+Δϕ^2 ). Jets are the signature of partons, materialized as sprays of highly collimated hadrons. A particle flow jet is the output of the jet finding algorithm when applied to a set of particle 4-vectors. A jet algorithm is a set of mathematical rules that reconstruct unambiguously the properties of a jet. Examples include Fixed Cone Algorithms like Iterative Cone and Seedless Infrared Safe Cone (SISCone), and Successive Recombination Algorithms. The latter is defined by d_ij=p_(T,i)^2p  and d_ij=min⁡(p_(T,i)^2p,p_(T,j)^2p )  (ΔR_ij^2)/D^2 . Now, p=-1,0,1 correspond to Anti-kT, CA, and kT jet algorithms respectively. 
Different inputs to the jet algorithm lead to different types of jets:
	Calorimeter jets (CaloJets): Clustered from CaloTowers
	Track Jets: Clustered from charged particle tracks
	Jets plus Tracks: Correct calorimeter jets using momentum of tracks.
	Particle Flow Jets: Clustered from identified particles, reconstructed using all detector components.
In CMS the most widely used jet is anti-kT 0.5 (0.7 for QCD measurements). For pileup studies, consider anti-kT 0.5, 0.7, 0.8 with various grooming techniques: filtering, trimming, pruning.
Jet substructure is currently a very popular tool to analyze jets that are produced from heavy objects such as top quarks, Higgs bosons, W/Z bosons, or any beyond-Standard-Model hadronically-decaying object. Jet pruning algorithm is designed to find heavy objects within a jet, and in the process, removes soft and wide-angle clusters from the clustering sequence. Traditional techniques start to lose sensitivity (in part) due to jet merging at higher masses. Therefore, we cannot rely on methods to assign partons to jets anymore and have to consider cases where partons merge into a single jet. We consider two types of jets:
	Top Jets
If a top quark or other heavy object is produced with enough energy its decay products can be reconstructed within one jet. Substructure can be used to identify these jets; top jets produce at least 3 sub-jets, where two of the sub-jets should have the W mass and third should have the top mass.
	W Jets
A partially merged boosted top results in a W jet and a b jet. W jets can be identified using jet and sub-jet properties:
	Jet mass = W mass
	Two sub-jets
	Sub-jet mass << jet mass
	Both sub-jets should have similar momentum
Jet cross section at LHC is several orders of magnitude higher than any other process. Therefore, we need to understand their performance as much as possible. The baseline jet object at CMS is the Particle Flow Jets. Jets need to be calibrated and cleaned before they can be used for physics analysis. The goal of this project is to use data driven methods and algorithms mentioned above to correct jet energies to the particle level and to use new data to probe new TeV regime.
