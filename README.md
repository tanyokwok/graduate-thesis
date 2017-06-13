# graduate-thesis
硕士毕业论文

#摘要
主题模型作为一种能够挖掘文本语义的技术受到了研究者的青睐,并且在业界得到了广泛的应用。在社交网络等领域中,主题模型是文本分类,检索以及推荐等应用的一项重要技术。
随着移动互联网的发展应用,社交网络等许多场景中数据的产生正呈现出越来越快的增长趋势。许多数据都具有高速、海量、实时、突发等主要特性。人们通常形象地将这类数据称为流式数据。
面对这种新型的数据流式特性,以往的主题模型的训练方法遭遇了巨大的挑战。流式机器学习的主要挑战在于,根据流式数据的特性,算法必须满足使用内存大小固定,高效实时,并且能够克服数据变动带来的对模型训练的影响。以往大部分的主题模型算法实现都采用了批量的学习方法,但是批量学习并不满足上述要求。
通过调研,本文发现流式主题模型的设计与实现的主要难题在于:(1) 流式数据具有海量无限的体量,并且数据分布时刻发生变化;(2) 在社交网络等类似的数据环境下,不断会有新词出现,词表是动态增长的;海量参数的分布式存储与并行更新同步困难;(3) 流式学习系统对算法实时性的要求极高;
本文主要工作是设计与实现高效的分布式流式主题模型,以应对上面提出的挑战。首先,本文提出了一种针对流式数据的在线流式主题模型。该模型能够有效地克服流式数据的无限性与变动性,不仅算法能够动态地更新模型,而且具有概念迁移的能力。然后,本文从算法实现的角度出发设计了稠密和稀疏并存的混合参数数据结构,解决了动态词表所带来的参数存储与更新的难题。最后,本文提出了一种新的采样方法,大大降低了采样的复杂度,并在此基础上进一步优化了算法的实现,保证了系统对算法实时性的要求。本文提出的分布式流式主题模型的实现是一种高效,实时的具有动态演化能力的主题模型。
