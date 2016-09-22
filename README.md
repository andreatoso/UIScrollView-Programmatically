# UIScrollView-Programmatically
Creating a UIScrollView using Autolayout (programmatically) with auto-height.

* Programmatic (no storyboard / nib)
* Autolayout
* UIScrollView
* ContentView inside UIScrollView
* Dynamic height
* Handles rotation

<b>Define UIScrollView & contentView</b></br>
  let scrollView = UIScrollView()</br>
  let contentView = UIView()
  
<b>Add constraints to scrollView</b></br>
  //x,w,t,b</br>
  scrollView.centerXAnchor.constraint(equalTo: view.centerXAnchor).isActive = true</br>
  scrollView.widthAnchor.constraint(equalTo: view.widthAnchor).isActive = true</br>
  scrollView.topAnchor.constraint(equalTo: view.topAnchor).isActive = true</br>
  scrollView.bottomAnchor.constraint(equalTo: view.bottomAnchor).isActive = true</br>
  
<b>Add constraints to contentView</b></br>
  //x,w,t,b</br>
  contentView.centerXAnchor.constraint(equalTo: scrollView.centerXAnchor).isActive = true</br>
  contentView.widthAnchor.constraint(equalTo: scrollView.widthAnchor).isActive = true</br>
  contentView.topAnchor.constraint(equalTo: scrollView.topAnchor).isActive = true</br>
  contentView.bottomAnchor.constraint(equalTo: scrollView.bottomAnchor).isActive = true</br>

<b>Add label to contentView and adding constraints</b></br>
  contentView.addSubview(label1)</br>
  label1.centerXAnchor.constraint(equalTo: contentView.centerXAnchor).isActive = true</br>
  label1.topAnchor.constraint(equalTo: contentView.topAnchor).isActive = true</br>
  label1.widthAnchor.constraint(equalTo: contentView.widthAnchor, multiplier: 3/4).isActive = true</br>
  label1.bottomAnchor.constraint(equalTo: contentView.bottomAnchor).isActive = true</br>
        
