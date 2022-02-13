# LiveData
in viewModel:
var word =  MutableLiveData<String>()

in view (fragment)
viewModel.score.observe(viewLifecycleOwner, Observer { newScore ->
    viewBinding.scoreText.text = newScore.toString()
