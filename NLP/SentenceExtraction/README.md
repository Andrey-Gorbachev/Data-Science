# Sentence Extraction

- используется датасет с русскими новостями collection5 и средства загрузки данных corus
- удаляем часто употребляемые слова common words (stoplist)
- формируем словарь  с помощью gensim.corpora.dictionary
- формируем BOW (Bag Of words) corpus слов
- тренируем ммодель gensim.models.ldamodel
- выводим topic (темы) данного корпуса, выученные LDA ( Latent Dirichlet Allocation )
- визуализируем pyLDAvis.display(vis_data)
- разбиваем корпус текстов на темы
- формируем  модель схожести текстов gensim.models.LsiModel
- формируем индекс схожести с помощью gensim.similarities
- выбираем темы вручную
- токенизируем и превращаем в векторы BOW и LSI (Latent Semantic Indexing)
- дополнительно  - формируем список похожих слов с помощью gensim.w2v.most_similar(positive=[token], topn=num_sim_words)] 
- сравниваем тексты по вручную выбранным темам с текстами, выученными LDA
