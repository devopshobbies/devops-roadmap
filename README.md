# DevOps-Roadmap

<p align="center">
 <img alt="DevOps Logo" src="image/DevOps.png">
</p>

## Step 1: (Basic requirements)
- Linux(LPIC-1)
- Docker
- Bash-Script
    - [Bash Script Tutorial](https://github.com/ahmadalibagheri/bash-script-tutorial) (Sample Traning Code)
- Git
    - [Git Learning with Jadi](https://faradars.org/courses/fvgit9609-git-github-gitlab) (Persian Language) 
    - [Git Learning with Mosh](https://codewithmosh.com/p/the-ultimate-git-course) (English Language) 
## Step 2: IaC (Infrastructure as Code)
- Terraform 
## Step 3:

## Published articles:

## Published articles:


# pictures_controller.rb
def upvote
  @picture = Picture.find(params[:id])
  @picture.liked_by current_user
  redirect_to @picture
end

def downvote
  @picture = Picture.find(params[:id])
  @picture.downvote_from current_user
  redirect_to @picture
end

# config/routes.rb

resources :pictures do
  member do
    put "like", to: "pictures#upvote"
    put "dislike", to: "pictures#downvote"
  end
end

# some view

<%= link_to "Upvote", like_picture_path(@picture), method: :put %>
<%= link_to "Downvote", dislike_picture_path(@picture), method: :put %>