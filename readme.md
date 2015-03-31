rails generate model Article title:string text:text


doc  ->   //https://github.com/activeadmin/activeadmin/blob/master/docs/0-installation.md



User: admin@example.com
Password: password




rails generate model Book image:string title:string author:string
rails generate active_admin:resource Book


buku



But first, an even smaller test. Could you create a base Rails app that uses ActiveAdmin to manage books?

Books should have a cover image, a title, and an author.

Then make a couple simple views where normal users can browse the books





====================


  controller do

    def create
      @book = Book.new(permit_params)
    end



    private
  def permit_params
    params.require(:article).permit(:image, :title, :author)
  end